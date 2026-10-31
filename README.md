# LaserData

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

LaserData is a hyper-efficient data streaming platform built in Rust for AI-native, real-time, and latency-sensitive workloads. Founded by the creators of Apache Iggy, LaserData packages the Iggy message-streaming engine — io_uring, thread-per-core, zero-copy deserialization, no garbage collection — as a managed cloud, BYOC, and on-premise product with sub-millisecond p99 latency and millions of messages per second per node. LaserData Cloud exposes a public REST control plane across three OpenAPI 3.1 services (Core, Audit, Notifier) covering tenants, divisions, environments, deployments, connectors, networking, API keys, roles and permissions, billing, notifications, and an immutable audit log, plus a per-deployment Supervisor API for configs, metrics, logs, diagnostic snapshots, and backups. The platform ships a first-party Rust SDK, a single-binary CLI with an interactive TUI, and an official Claude Code Agent Skill pack.

**Areas:** Streaming · Message Streaming · Event Streaming · Data Infrastructure · Real-Time · Apache Iggy · Rust · Cloud Infrastructure · AI Agents · Observability · Company

## LaserData on APIs.io

Everything profiled for LaserData is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/laserdata/](https://apis.io/providers/laserdata/)** — or go straight to one of the APIs or properties below.

### APIs (18)

- [LaserData Account API](https://apis.io/apis/laserdata/laserdata-account-api/) — User account, sign-in, sessions, settings
- [LaserData API Keys API](https://apis.io/apis/laserdata/laserdata-api-keys-api/) — Tenant API key management
- [LaserData Audit API](https://apis.io/apis/laserdata/laserdata-audit-api/) — Tenant audit log + user activity
- [LaserData Billing API](https://apis.io/apis/laserdata/laserdata-billing-api/) — Pricing, billing reports, invoices
- [LaserData Cloud Accounts API](https://apis.io/apis/laserdata/laserdata-cloud-accounts-api/) — BYOC cloud accounts
- [LaserData Clouds API](https://apis.io/apis/laserdata/laserdata-clouds-api/) — Available clouds, regions, clusters, storages, tiers
- [LaserData Connectors API](https://apis.io/apis/laserdata/laserdata-connectors-api/) — Deployment connectors
- [LaserData Deployments API](https://apis.io/apis/laserdata/laserdata-deployments-api/) — Deployment lifecycle
- [LaserData Divisions API](https://apis.io/apis/laserdata/laserdata-divisions-api/) — Tenant divisions
- [LaserData Environments API](https://apis.io/apis/laserdata/laserdata-environments-api/) — Environments within a division
- [LaserData Invitations API](https://apis.io/apis/laserdata/laserdata-invitations-api/) — Tenant invitations
- [LaserData Members API](https://apis.io/apis/laserdata/laserdata-members-api/) — Tenant members
- [LaserData Notification Channels API](https://apis.io/apis/laserdata/laserdata-notification-channels-api/) — Notification channels (email, slack, webhook)
- [LaserData Notification Subscriptions API](https://apis.io/apis/laserdata/laserdata-notification-subscriptions-api/) — Channel subscriptions to notification types
- [LaserData Notifications API](https://apis.io/apis/laserdata/laserdata-notifications-api/) — Notifications listing
- [LaserData Payments API](https://apis.io/apis/laserdata/laserdata-payments-api/) — Payment methods (Stripe)
- [LaserData Roles API](https://apis.io/apis/laserdata/laserdata-roles-api/) — Tenant roles and permissions
- [LaserData Tenants API](https://apis.io/apis/laserdata/laserdata-tenants-api/) — Tenant CRUD, config, structure

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Laserdata Notifications Webhooks](https://apis.io/asyncapis/laserdata/laserdata-notifications-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [laserdata](https://apis.io/servers/laserdata/laserdata/)

#### Collections (18)

Postman and Open Collection request collections.

- [LaserData Cloud Audit Account API](https://apis.io/collections/laserdata/open-laserdata-account-api/)
- [LaserData Cloud Audit Account API Keys API](https://apis.io/collections/laserdata/open-laserdata-api-keys-api/)
- [LaserData Cloud Account Audit API](https://apis.io/collections/laserdata/open-laserdata-audit-api/)
- [LaserData Cloud Audit Account Billing API](https://apis.io/collections/laserdata/open-laserdata-billing-api/)
- [LaserData Cloud Audit Account Cloud Accounts API](https://apis.io/collections/laserdata/open-laserdata-cloud-accounts-api/)
- [LaserData Cloud Audit Account Clouds API](https://apis.io/collections/laserdata/open-laserdata-clouds-api/)
- [LaserData Cloud Audit Account Connectors API](https://apis.io/collections/laserdata/open-laserdata-connectors-api/)
- [LaserData Cloud Audit Account Deployments API](https://apis.io/collections/laserdata/open-laserdata-deployments-api/)
- [LaserData Cloud Audit Account Divisions API](https://apis.io/collections/laserdata/open-laserdata-divisions-api/)
- [LaserData Cloud Audit Account Environments API](https://apis.io/collections/laserdata/open-laserdata-environments-api/)
- [LaserData Cloud Audit Account Invitations API](https://apis.io/collections/laserdata/open-laserdata-invitations-api/)
- [LaserData Cloud Audit Account Members API](https://apis.io/collections/laserdata/open-laserdata-members-api/)
- [LaserData Cloud Audit Account Notification Channels API](https://apis.io/collections/laserdata/open-laserdata-notification-channels-api/)
- [LaserData Cloud Audit Account Notification Subscriptions API](https://apis.io/collections/laserdata/open-laserdata-notification-subscriptions-api/)
- [LaserData Cloud Audit Account Notifications API](https://apis.io/collections/laserdata/open-laserdata-notifications-api/)
- [LaserData Cloud Audit Account Payments API](https://apis.io/collections/laserdata/open-laserdata-payments-api/)
- [LaserData Cloud Audit Account Roles API](https://apis.io/collections/laserdata/open-laserdata-roles-api/)
- [LaserData Cloud Audit Account Tenants API](https://apis.io/collections/laserdata/open-laserdata-tenants-api/)

#### Overlays (3)

OpenAPI overlays, including conversational phrasing for each operation.

- [Laserdata Audit Overlay](https://apis.io/overlays/laserdata/laserdata-audit-overlay/)
- [Laserdata Core Overlay](https://apis.io/overlays/laserdata/laserdata-core-overlay/)
- [Laserdata Notifier Overlay](https://apis.io/overlays/laserdata/laserdata-notifier-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Laserdata Authentication](https://apis.io/security/laserdata/laserdata-authentication/)
- [Laserdata Domain Security](https://apis.io/security/laserdata/laserdata-domain-security/)
- [Laserdata Vulnerability Disclosure](https://apis.io/security/laserdata/laserdata-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://laserdata.com)
- [Documentation](https://docs.laserdata.cloud)
- [Getting started](https://docs.laserdata.cloud/getting-started/quick-start)
- [API reference](https://api.laserdata.cloud/docs)
- [Sign up](https://laserdata.cloud)
- [Blog](https://laserdata.com/blog)
- [Security](https://github.com/laserdata/laser-sdk/blob/main/SECURITY.md)
- [Terms of service](https://laserdata.com/terms)
- [Privacy policy](https://laserdata.com/privacy-policy)
- [GitHub](https://github.com/laserdata)
- [Status](https://status.laserdata.cloud)

## API Evangelist rating

**Kin Score 58.3** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 62.1 |
| Contract governance | 4.5 |
| Operational transparency | 44.7 |
| Developer ergonomics | 86.9 |
| Access clarity | 34.2 |

**Agent readiness 28.9** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | derived (partial credit) |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 30.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/laserdata/](https://apis.io/providers/laserdata/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for LaserData: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/laserdata/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
