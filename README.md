# Lever (lever)

Lever is a talent acquisition and applicant tracking platform built on the Opportunities data model. The Lever API exposes candidates, opportunities, postings, interviews, feedback, requisitions, users, files, webhooks, and a public Postings API for embedding job sites.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/lever/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/lever/refs/heads/main/apis.yml)

## Tags

- HR
- ATS
- Recruiting
- Talent Acquisition
- SaaS

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-19

## APIs

### Lever Opportunities API

Opportunities are Lever's primary candidate-centric resource. List, create, advance, archive, and update candidate opportunities through the hiring pipeline. Replaces the legacy Candidates resource.

#### Tags

- Opportunities
- Candidates
- Pipeline

#### Properties

- [OpenAPI](openapi/lever-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://hire.lever.co/developer/documentation#opportunities)
- [API Reference](https://hire.lever.co/developer/documentation)

### Lever Candidates API

Legacy Candidates endpoints maintained for backward compatibility. New integrations should use Opportunities; Candidates remain available for historical record retrieval.

#### Tags

- Candidates
- Legacy

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#candidates)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Contacts API

Contacts represent unique people across multiple opportunities, allowing Lever to deduplicate candidates who apply to multiple roles.

#### Tags

- Contacts
- People

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#contacts)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Postings API

Manage job postings programmatically and power custom public job sites. The Postings API has a public read-only mode that does not require authentication for displaying job listings.

#### Tags

- Postings
- Jobs
- Public

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#postings)
- [SDK](https://github.com/lever/postings-api)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Applications API

Submit candidate applications against postings, including resumes, cover letters, and EEO survey data, and retrieve historical application records.

#### Tags

- Applications
- Submissions

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#applications)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Stages API

List the configured pipeline stages and disposition stages used to route opportunities through screening, interviews, offer, and hire.

#### Tags

- Stages
- Pipeline

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#stages)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Archive Reasons API

Read archive reasons used when an opportunity is archived (rejected, hired, withdrawn) for downstream EEO and analytics reporting.

#### Tags

- Archive Reasons
- Disposition

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#archive-reasons)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Interviews API

Read interview events, panels, and schedules associated with an opportunity, including interviewer assignments and time slots.

#### Tags

- Interviews
- Panels
- Scheduling

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#interviews)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Feedback API

Read feedback forms and scorecards completed by interviewers and hiring managers, with templated and free-form fields.

#### Tags

- Feedback
- Scorecards

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#feedback)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Feedback Templates API

Manage feedback form templates, including question definitions and scoring rubrics applied across postings and stages.

#### Tags

- Feedback Templates
- Forms

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#feedback-templates)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Notes API

Add and retrieve free-form notes attached to opportunities for recruiter and hiring manager collaboration.

#### Tags

- Notes

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#notes)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Offers API

Read offer records associated with opportunities, including offer letters, approval status, and compensation breakdowns.

#### Tags

- Offers
- Approvals

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#offers)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Requisitions API

Manage requisitions backing each posting — headcount, compensation bands, and approval state — typically synced from an HRIS.

#### Tags

- Requisitions
- Headcount

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#requisitions)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Tags API

List and apply tags to opportunities for cohorting, sourcing, and reporting workflows.

#### Tags

- Tags
- Metadata

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#tags)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Sources API

Read source attribution (job board, referral, sourced) for opportunities to drive sourcing analytics.

#### Tags

- Sources
- Attribution

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#sources)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Files API

Upload and download files (resumes, cover letters, portfolio attachments) associated with opportunities; supports docx, doc, pdf, txt, jpg, png.

#### Tags

- Files
- Resumes

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#files)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Resumes API

Read parsed resume data — work history, education, skills — extracted from candidate submissions.

#### Tags

- Resumes
- Parsing

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#resumes)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Users API

Manage Lever users and their access roles (Super Admin, Admin, Team Member, Limited Team Member, Interviewer, Outsider).

#### Tags

- Users
- Permissions

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#users)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Audit Events API

Read tenant-scoped audit events for security monitoring and SOC reporting.

#### Tags

- Audit
- Security

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#audit-events)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever EEO API

Read anonymous EEO survey data for compliance reporting; PII-isolated from the standard candidate endpoints.

#### Tags

- EEO
- Compliance

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#eeo)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Webhooks API

Subscribe to Lever events (applicationCreated, candidateHired, stageChange, contactUpdate). Events are signed with HMAC-SHA256 for receiver verification.

#### Tags

- Webhooks
- Events

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#webhooks)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever Postings Public API

The unauthenticated public Postings API for retrieving live job listings from a Lever account, used by external careers pages.

#### Tags

- Postings
- Public
- Jobs

#### Properties

- [Documentation](https://github.com/lever/postings-api)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lever XML Feed

XML feed of open postings used by job aggregators (Indeed, Glassdoor, LinkedIn) for syndication.

#### Tags

- XML
- Job Boards
- Aggregators

#### Properties

- [Documentation](https://hire.lever.co/developer/documentation#xml-feed)
- [Postman Collection](collections/lever.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lever.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/lever-)
- [Website](https://www.lever.co/)
- [Documentation](https://hire.lever.co/developer)
- [API Reference](https://hire.lever.co/developer/documentation)
- [Pricing](https://www.lever.co/pricing/)
- [Login](https://hire.lever.co/login)
- [Status Page](https://status.lever.co/)
- [Blog](https://www.lever.co/blog)
- [Support](https://help.lever.co/)
- [GitHub Organization](https://github.com/lever)
- [Privacy Policy](https://www.lever.co/privacy/)
- [Terms of Service](https://www.lever.co/legal/)
- [Authentication](https://hire.lever.co/developer/oauth)
- [Webhooks](https://hire.lever.co/developer/documentation#webhooks)
- [Plans](plans/lever-plans-pricing.yml)
- [Rate Limits](rate-limits/lever-rate-limits.yml)
- [Fin Ops](finops/lever-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
