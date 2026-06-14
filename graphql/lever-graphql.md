# Lever GraphQL Schema

## Overview

This document describes a conceptual GraphQL schema for the Lever ATS (Applicant Tracking System) API. Lever's production API is REST-based (https://api.lever.co/v1), but this schema translates the full breadth of Lever's data model — opportunities, candidates, postings, interviews, feedback, offers, requisitions, users, webhooks, and compliance resources — into a typed GraphQL surface.

The schema is derived from the Lever Developer Documentation at https://hire.lever.co/developer/documentation and covers the Opportunities data model that is central to Lever's architecture.

## Schema Source

- Provider: Lever
- API Reference: https://hire.lever.co/developer/documentation
- GitHub: https://github.com/lever
- Schema type: Conceptual (REST-to-GraphQL translation)
- Schema file: lever-schema.graphql

## Core Data Model

Lever's data model is organized around the **Opportunity**, which is the primary candidate-centric resource. Each Opportunity represents a single candidate's journey through a hiring pipeline for a specific Posting. Key relationships:

- An **Opportunity** belongs to a **Contact** (the unique person record) and a **Posting** (the job).
- Opportunities move through **PipelineStages** and can be **archived** with an **ArchiveReason**.
- **Interviews** and **Panels** are attached to Opportunities; interviewers submit **Feedback** (scorecards).
- **Offers** with approval workflows are attached to Opportunities.
- **Requisitions** back Postings and track headcount.
- **Webhooks** deliver signed event payloads for real-time integrations.

## Types (62 Named Types)

### Candidate and Pipeline

| Type | Description |
|------|-------------|
| Opportunity | Central candidate-in-pipeline record replacing the legacy Candidate resource |
| Application | Formal submission of a candidate against a Posting, with resume and form data |
| Resume | Parsed resume data including work history, education, and skills |
| Stage | Current pipeline stage of an Opportunity (screening, interview, offer, etc.) |
| PipelineStage | Configured stage definition in a Lever account's hiring pipeline |
| Archive | Record of an Opportunity being removed from active pipeline |
| ArchiveReason | Reason code for archival (rejected, hired, withdrawn, declined) |
| Tag | Label applied to Opportunities for cohorting and reporting |
| Source | Attribution source for how a candidate entered the pipeline |
| Attribution | Full attribution record linking Source and channel to an Opportunity |

### Interviews and Feedback

| Type | Description |
|------|-------------|
| InterviewPanel | A scheduled panel or interview loop tied to an Opportunity |
| Interview | A single interview event within a Panel, with time slot and location |
| InterviewFeedback | Feedback record submitted by an interviewer for an Interview |
| Scorecard | Structured scorecard with scored dimensions and an overall recommendation |
| FeedbackTemplate | Template defining questions and scoring rubrics for a stage or posting |
| FormField | A single field definition within a FeedbackTemplate or PostingForm |
| Panel | Grouping of interviewers assigned to an Interview event |

### Offers and Approvals

| Type | Description |
|------|-------------|
| Offer | Offer record attached to an Opportunity, with compensation and status |
| OfferVersion | Versioned snapshot of an Offer, capturing changes over approval cycles |
| OfferApproval | Individual approval step in an Offer approval chain |

### Jobs and Postings

| Type | Description |
|------|-------------|
| Posting | Job listing with title, description, requirements, and application form |
| PostingForm | Application form attached to a Posting with custom fields |
| PostingApplication | A candidate's application submission through a Posting's public form |
| JobLocation | Location (city, state, country, remote flag) attached to a Posting |
| JobWorkType | Work type classification (full-time, part-time, contract, internship) |
| AnonymousLink | Shareable link for a Posting that does not expose the candidate's identity |
| ReferralForm | Employee referral submission form attached to a Posting |

### Requisitions and Organization

| Type | Description |
|------|-------------|
| Requisition | Headcount request backing a Posting, with compensation bands and approval state |
| Department | Organizational department grouping Postings and Requisitions |
| Team | Sub-group within a Department for finer-grained reporting |
| HiringManager | User designated as Hiring Manager on an Opportunity or Posting |

### People

| Type | Description |
|------|-------------|
| Contact | Unique person record deduplicating candidates across multiple Opportunities |
| ContactEmail | Email address associated with a Contact |
| ContactPhone | Phone number associated with a Contact |
| User | Lever platform user with a role (Super Admin, Admin, Team Member, Interviewer, Outsider) |
| HiringTeam | Collection of Users assigned roles on an Opportunity (coordinator, recruiter, hiring manager) |

### Notes and Communication

| Type | Description |
|------|-------------|
| InternalNote | Private note on an Opportunity visible only to hiring team members |
| ExternalNote | Note on an Opportunity that can be shared externally |

### Surveys and Data Protection

| Type | Description |
|------|-------------|
| SurveySend | Record of a survey being sent to a candidate |
| SurveyResponse | Candidate's response to a survey |
| SurveyQuestion | Individual question within a Survey |
| DataProtection | GDPR/data protection settings for a Contact or Opportunity |
| ConsentRequest | Consent request sent to a candidate for data processing |

### Webhooks and Events

| Type | Description |
|------|-------------|
| Webhook | Registered webhook subscription (endpoint URL, event types, signing secret) |
| WebhookEvent | Delivered webhook event payload with signature and status |

### Authentication and Platform

| Type | Description |
|------|-------------|
| APIToken | API key or OAuth token used to authenticate API requests |
| OAuthClient | Registered OAuth 2.0 client application |
| Organization | Lever tenant/account configuration |
| Pipeline | Named hiring pipeline configuration for a Posting or account |
| FeedbackToken | Time-limited token allowing an interviewer to submit feedback without a Lever login |
| AuditEvent | Tenant-scoped audit log entry for security monitoring |
| EEOData | Anonymous Equal Employment Opportunity survey data for compliance reporting |
| XMLFeedEntry | Entry in the XML job aggregator feed (Indeed, Glassdoor, LinkedIn) |

## Queries

- `opportunity(id: ID!)`: Fetch a single Opportunity by ID
- `opportunities(filter: OpportunityFilter, limit: Int, cursor: String)`: Paginated list of Opportunities
- `contact(id: ID!)`: Fetch a Contact by ID
- `contacts(filter: ContactFilter, limit: Int, cursor: String)`: Paginated list of Contacts
- `posting(id: ID!)`: Fetch a Posting by ID
- `postings(filter: PostingFilter, limit: Int, cursor: String)`: List Postings (supports unauthenticated public mode)
- `stage(id: ID!)`: Fetch a Stage definition
- `stages`: List all configured pipeline stages
- `archiveReasons`: List all archive reason codes
- `user(id: ID!)`: Fetch a User by ID
- `users(filter: UserFilter, limit: Int, cursor: String)`: List Users
- `requisition(id: ID!)`: Fetch a Requisition by ID
- `requisitions(filter: RequisitionFilter, limit: Int, cursor: String)`: List Requisitions
- `interview(id: ID!)`: Fetch an Interview by ID
- `interviews(opportunityId: ID!)`: List Interviews for an Opportunity
- `offer(id: ID!)`: Fetch an Offer by ID
- `webhooks`: List registered Webhook subscriptions
- `auditEvents(filter: AuditEventFilter, limit: Int, cursor: String)`: List Audit Events

## Mutations

- `createOpportunity(input: CreateOpportunityInput!)`: Create a new Opportunity
- `updateOpportunity(id: ID!, input: UpdateOpportunityInput!)`: Update an Opportunity
- `archiveOpportunity(id: ID!, reasonId: ID!)`: Archive an Opportunity
- `advanceOpportunity(id: ID!, stageId: ID!)`: Move Opportunity to a new stage
- `createNote(opportunityId: ID!, input: CreateNoteInput!)`: Add a note to an Opportunity
- `createPosting(input: CreatePostingInput!)`: Create a new Posting
- `updatePosting(id: ID!, input: UpdatePostingInput!)`: Update a Posting
- `createApplication(input: CreateApplicationInput!)`: Submit a candidate application
- `createOffer(opportunityId: ID!, input: CreateOfferInput!)`: Create an Offer
- `approveOffer(offerId: ID!)`: Approve an Offer in the approval chain
- `createRequisition(input: CreateRequisitionInput!)`: Create a Requisition
- `createWebhook(input: CreateWebhookInput!)`: Register a Webhook subscription
- `deleteWebhook(id: ID!)`: Remove a Webhook subscription
- `createUser(input: CreateUserInput!)`: Invite a new User
- `updateUser(id: ID!, input: UpdateUserInput!)`: Update a User's role or details
- `addTagToOpportunity(opportunityId: ID!, tag: String!)`: Tag an Opportunity

## Authentication

The Lever REST API supports Basic Auth (API key as username, empty password) and OAuth 2.0 for partner applications. A conceptual GraphQL implementation would accept:

- `Authorization: Basic <base64(apiKey:)>` for internal integrations
- `Authorization: Bearer <access_token>` for OAuth 2.0 partner apps

Rate limits: 10 requests/second per API key with burst to 20 req/s (token bucket model).

## Pagination

Lever uses cursor-based pagination with `limit` (1-100) and `offset` token parameters. This schema represents that as a `Connection` pattern with `cursor` and `limit` arguments and a `PageInfo` type with `hasNextPage` and `nextCursor` fields.
