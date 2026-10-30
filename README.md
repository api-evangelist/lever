# Lever

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
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

**Areas:** Human Resources · Applicant Tracking · Recruiting · Talent Acquisition · Software-as-a-Service

## Lever on APIs.io

Everything profiled for Lever is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/lever/](https://apis.io/providers/lever/)** — or go straight to one of the APIs or properties below.

### APIs (24)

- [Lever Candidates API](https://apis.io/apis/lever/lever-candidates-api/) — Legacy Candidates endpoints maintained for backward compatibility. New integrations should use Opportunities; Candidates remain available for historical…
- [Lever Feedback Templates API](https://apis.io/apis/lever/lever-feedback-templates-api/) — Manage feedback form templates, including question definitions and scoring rubrics applied across postings and stages.
- [Lever Webhooks API](https://apis.io/apis/lever/lever-webhooks-api/) — Subscribe to Lever events (applicationCreated, candidateHired, stageChange, contactUpdate). Events are signed with HMAC-SHA256 for receiver verification.
- [Lever Postings Public API](https://apis.io/apis/lever/lever-postings-public-api/) — The unauthenticated public Postings API for retrieving live job listings from a Lever account, used by external careers pages.
- [Lever XML Feed](https://apis.io/apis/lever/lever-xml-feed-api/) — XML feed of open postings used by job aggregators (Indeed, Glassdoor, LinkedIn) for syndication.
- [Lever Applications API](https://apis.io/apis/lever/lever-applications-api/) — Submit candidate applications against postings, including resumes, cover letters, and EEO survey data, and retrieve historical application records.
- [Lever Contacts API](https://apis.io/apis/lever/lever-contacts-api/) — Contacts represent unique people across multiple opportunities, allowing Lever to deduplicate candidates who apply to multiple roles.
- [Lever EEO API](https://apis.io/apis/lever/lever-eeo-api/) — Read anonymous EEO survey data for compliance reporting; PII-isolated from the standard candidate endpoints.
- [Lever Feedback API](https://apis.io/apis/lever/lever-feedback-api/) — Read feedback forms and scorecards completed by interviewers and hiring managers, with templated and free-form fields.
- [Lever Files API](https://apis.io/apis/lever/lever-files-api/) — Upload and download files (resumes, cover letters, portfolio attachments) associated with opportunities; supports docx, doc, pdf, txt, jpg, png.
- [Lever Forms API](https://apis.io/apis/lever/lever-forms-api/) — The Forms API from Lever — 2 operation(s) for forms.
- [Lever Interviews API](https://apis.io/apis/lever/lever-interviews-api/) — Read interview events, panels, and schedules associated with an opportunity, including interviewer assignments and time slots.
- [Lever Notes API](https://apis.io/apis/lever/lever-notes-api/) — Add and retrieve free-form notes attached to opportunities for recruiter and hiring manager collaboration.
- [Lever Offers API](https://apis.io/apis/lever/lever-offers-api/) — Read offer records associated with opportunities, including offer letters, approval status, and compensation breakdowns.
- [Lever Opportunities API](https://apis.io/apis/lever/lever-opportunities-api/) — The Opportunities API from Lever — 10 operation(s) for opportunities.
- [Lever Postings API](https://apis.io/apis/lever/lever-postings-api/) — Manage job postings programmatically and power custom public job sites. The Postings API has a public read-only mode that does not require authentication…
- [Lever Requisitions API](https://apis.io/apis/lever/lever-requisitions-api/) — Manage requisitions backing each posting — headcount, compensation bands, and approval state — typically synced from an HRIS.
- [Lever Resumes API](https://apis.io/apis/lever/lever-resumes-api/) — Read parsed resume data — work history, education, skills — extracted from candidate submissions.
- [Lever Sources API](https://apis.io/apis/lever/lever-sources-api/) — Read source attribution (job board, referral, sourced) for opportunities to drive sourcing analytics.
- [Lever Stages API](https://apis.io/apis/lever/lever-stages-api/) — List the configured pipeline stages and disposition stages used to route opportunities through screening, interviews, offer, and hire.
- [Lever Tags API](https://apis.io/apis/lever/lever-tags-api/) — List and apply tags to opportunities for cohorting, sourcing, and reporting workflows.
- [Lever Users API](https://apis.io/apis/lever/lever-users-api/) — Manage Lever users and their access roles (Super Admin, Admin, Team Member, Limited Team Member, Interviewer, Outsider).
- [Lever Archive Reasons API](https://apis.io/apis/lever/lever-archive-reasons-api/) — The Archive Reasons API from Lever — 2 operation(s) for archive reasons.
- [Lever Audit Events API](https://apis.io/apis/lever/lever-audit-events-api/) — The Audit Events API from Lever — 1 operation(s) for audit events.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/lever/](https://apis.io/graphqls/lever/lever-graphql/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Lever Agentic Access](https://apis.io/agentic-access/lever/lever-agentic-access/)

#### Collections (20)

Postman and Open Collection request collections.

- [Lever API](https://apis.io/collections/lever/open-lever/)
- [Lever Applications API](https://apis.io/collections/lever/open-lever-applications-api/)
- [Lever Applications ArchiveReasons API](https://apis.io/collections/lever/open-lever-archivereasons-api/)
- [Lever Applications AuditEvents API](https://apis.io/collections/lever/open-lever-auditevents-api/)
- [Lever Applications Contacts API](https://apis.io/collections/lever/open-lever-contacts-api/)
- [Lever Applications EEO API](https://apis.io/collections/lever/open-lever-eeo-api/)
- [Lever Applications Feedback API](https://apis.io/collections/lever/open-lever-feedback-api/)
- [Lever Applications Files API](https://apis.io/collections/lever/open-lever-files-api/)
- [Lever Applications Forms API](https://apis.io/collections/lever/open-lever-forms-api/)
- [Lever Applications Interviews API](https://apis.io/collections/lever/open-lever-interviews-api/)
- [Lever Applications Notes API](https://apis.io/collections/lever/open-lever-notes-api/)
- [Lever Applications Offers API](https://apis.io/collections/lever/open-lever-offers-api/)
- [Lever Applications Opportunities API](https://apis.io/collections/lever/open-lever-opportunities-api/)
- [Lever Applications Postings API](https://apis.io/collections/lever/open-lever-postings-api/)
- [Lever Applications Requisitions API](https://apis.io/collections/lever/open-lever-requisitions-api/)
- [Lever Applications Resumes API](https://apis.io/collections/lever/open-lever-resumes-api/)
- [Lever Applications Sources API](https://apis.io/collections/lever/open-lever-sources-api/)
- [Lever Applications Stages API](https://apis.io/collections/lever/open-lever-stages-api/)
- [Lever Applications Tags API](https://apis.io/collections/lever/open-lever-tags-api/)
- [Lever Applications Users API](https://apis.io/collections/lever/open-lever-users-api/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Lever Authentication](https://apis.io/security/lever/lever-authentication/)
- [Lever Domain Security](https://apis.io/security/lever/lever-domain-security/)
- [Lever Trust Center](https://apis.io/security/lever/lever-trust-center/)
- [Lever Vulnerability Disclosure](https://apis.io/security/lever/lever-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Lever Plans Pricing](https://apis.io/plans/lever/lever-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Lever Rate Limits](https://apis.io/rate-limits/lever/lever-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Lever Finops](https://apis.io/finops/lever/lever-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.lever.co/)
- [Documentation](https://hire.lever.co/developer)
- [API reference](https://hire.lever.co/developer/documentation)
- [Pricing](https://www.lever.co/pricing/)
- [Support](https://help.lever.co/)
- [Blog](https://www.lever.co/blog)
- [Terms of service](https://www.lever.co/legal/)
- [Privacy policy](https://www.lever.co/privacy/)
- [GitHub](https://github.com/lever)
- [Status](https://status.lever.co/)

## API Evangelist rating

**Kin Score 35.3** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 53.6 |
| Contract quality | 47.2 |
| Contract governance | 0.0 |
| Operational transparency | 26.3 |
| Developer ergonomics | 14.3 |
| Access clarity | 53.9 |

**Agent readiness 21.8** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | unknown |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 30.4** — Employment & Payroll

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/lever/](https://apis.io/providers/lever/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Lever: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/lever/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
