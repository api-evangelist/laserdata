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

LaserData is a hyper-efficient data streaming platform built in Rust for AI-native, real-time, and
latency-sensitive workloads. Founded by the creators of Apache Iggy, LaserData packages the Iggy
message-streaming engine — io_uring, thread-per-core, zero-copy deserialization, no garbage
collection — as a managed cloud, BYOC, and on-premise product with sub-millisecond p99 latency.

- Website: https://laserdata.com
- Documentation: https://docs.laserdata.cloud
- API reference: https://api.laserdata.cloud/docs
- Status: https://status.laserdata.cloud
- GitHub: https://github.com/laserdata

## APIs

LaserData Cloud publishes three OpenAPI 3.1 documents for its public REST control plane, plus a
per-deployment Supervisor API (authenticated, one spec per cloud/region pair).

| API | Base URL | Operations |
|---|---|---|
| Core — tenants, divisions, environments, deployments, connectors, API keys, roles, members, billing | `https://api.laserdata.cloud` | 95 |
| Audit — immutable audit log and per-user activity feed | `https://audit.laserdata.cloud` | 3 |
| Notifier — notification channels, subscriptions, delivery | `https://api.laserdata.cloud` | 26 |

Authentication is an `ld-api-key` header bound to a role; there are no OAuth flows.

## Artifacts

| Directory | What it holds |
|---|---|
| `openapi/` | The three published OpenAPI 3.1 specs, verbatim |
| `overlays/` | API Evangelist enhancement overlays (Overlay 1.0.0) |
| `skills/` | LaserData's own 14 published Claude Code Agent Skills, verbatim |
| `packages/` | First-party Rust SDK, Python bindings, CLI binary, quickstart image |
| `cli/` | The `laser` CLI command surface |
| `authentication/` | Auth profile plus the role/permission model |
| `conventions/` | Idempotency, pagination, tracing, rate-limit and error semantics |
| `errors/` | RFC 7807 problem catalogue derived from the specs |
| `data-model/` | Entity graph derived from spec schemas |
| `asyncapi/` | Notifier webhook catalogue (41 event types) — no AsyncAPI published |
| `sandbox/` | Free Tier and the quickstart producer/consumer harness |
| `lifecycle/` | Versioning, status page, credential lifecycle |
| `changelog/` | Release train across SDK, CLI and spec versions |
| `conformance/` | Standards conformance derived from the specs |
| `security/` | Domain security probe and vulnerability disclosure policy |
| `well-known/` | `/.well-known/` probe results (verified absence) |
| `mcp/` | Candidate MCP tool surface derived from OpenAPI (no hosted server published) |
| `llms/` | The provider's own `llms.txt`, verbatim |

Backed by: battery-ventures
