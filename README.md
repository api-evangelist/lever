# Lever (lever)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
