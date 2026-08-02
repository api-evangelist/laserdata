# LaserData

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
