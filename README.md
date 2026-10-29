# ClickHouse

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

ClickHouse is a fast open-source column-oriented database management system that enables real-time analytical reporting using SQL. ClickHouse exposes multiple interfaces - an HTTP interface for SQL queries, native TCP, MySQL and PostgreSQL wire-compatible interfaces, and a gRPC interface - and the ClickHouse Cloud management plane offers a public OpenAPI-described REST API for provisioning and managing services, organizations, members, API keys, backups, and private endpoints.

**Areas:** ClickHouse · Analytics · Cloud Database · Column-Oriented · Database · OLAP · Open Source · Real-Time · SQL

## ClickHouse on APIs.io

Everything profiled for ClickHouse is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/clickhouse/](https://apis.io/providers/clickhouse/)** — or go straight to one of the APIs or properties below.

### APIs (21)

- [ClickHouse HTTP Interface](https://apis.io/apis/clickhouse/clickhouse-http-interface/) — HTTP interface (default port 8123, HTTPS 8443) for executing SQL queries against ClickHouse. Supports SELECT via GET, mutations via POST, multiple output…
- [ClickHouse Native TCP Interface](https://apis.io/apis/clickhouse/clickhouse-native/) — Native binary TCP protocol used by ClickHouse client libraries for maximum throughput between client and server (default port 9000).
- [ClickHouse MySQL Interface](https://apis.io/apis/clickhouse/clickhouse-mysql/) — MySQL wire protocol compatibility allowing existing MySQL clients and BI tools to query ClickHouse without driver changes.
- [ClickHouse PostgreSQL Interface](https://apis.io/apis/clickhouse/clickhouse-postgresql/) — PostgreSQL wire protocol compatibility for connecting psql, JDBC and other PostgreSQL clients to ClickHouse.
- [ClickHouse gRPC Interface](https://apis.io/apis/clickhouse/clickhouse-grpc/) — gRPC interface defined by clickhouse_grpc.proto for efficient binary communication.
- [ClickHouse HTTP Interface API](https://apis.io/apis/clickhouse/clickhouse-clickhouse-http-interface-api/) — The ClickHouse HTTP Interface API from ClickHouse — 1 operation(s) for clickhouse http interface.
- [ClickHouse Ping API](https://apis.io/apis/clickhouse/clickhouse-ping-api/) — The Ping API from ClickHouse — 1 operation(s) for ping.
- [ClickHouse Play API](https://apis.io/apis/clickhouse/clickhouse-play-api/) — The Play API from ClickHouse — 1 operation(s) for play.
- [ClickHouse Replicas Status API](https://apis.io/apis/clickhouse/clickhouse-replicas-status-api/) — The Replicas Status API from ClickHouse — 1 operation(s) for replicas status.
- [ClickHouse API keys API](https://apis.io/apis/clickhouse/clickhouse-api-keys-api/) — The API keys API from ClickHouse — 2 operation(s) for api keys.
- [ClickHouse Backup API](https://apis.io/apis/clickhouse/clickhouse-backup-api/) — The Backup API from ClickHouse — 4 operation(s) for backup.
- [ClickHouse Billing API](https://apis.io/apis/clickhouse/clickhouse-billing-api/) — The Billing API from ClickHouse — 3 operation(s) for billing.
- [ClickHouse Click Pipes API](https://apis.io/apis/clickhouse/clickhouse-clickpipes-api/) — The ClickPipes API from ClickHouse — 10 operation(s) for clickpipes.
- [ClickHouse Click Stack API](https://apis.io/apis/clickhouse/clickhouse-clickstack-api/) — The ClickStack API from ClickHouse — 13 operation(s) for clickstack.
- [ClickHouse Organization API](https://apis.io/apis/clickhouse/clickhouse-organization-api/) — The Organization API from ClickHouse — 9 operation(s) for organization.
- [ClickHouse Postgres API](https://apis.io/apis/clickhouse/clickhouse-postgres-api/) — The Postgres API from ClickHouse — 12 operation(s) for postgres.
- [ClickHouse Prometheus API](https://apis.io/apis/clickhouse/clickhouse-prometheus-api/) — The Prometheus API from ClickHouse — 5 operation(s) for prometheus.
- [ClickHouse Role Management API](https://apis.io/apis/clickhouse/clickhouse-role-management-api/) — The Role Management API from ClickHouse — 2 operation(s) for role management.
- [ClickHouse Service API](https://apis.io/apis/clickhouse/clickhouse-service-api/) — The Service API from ClickHouse — 15 operation(s) for service.
- [ClickHouse UDF API](https://apis.io/apis/clickhouse/clickhouse-udf-api/) — The UDF API from ClickHouse — 7 operation(s) for udf.
- [ClickHouse User management API](https://apis.io/apis/clickhouse/clickhouse-user-management-api/) — The User management API from ClickHouse — 4 operation(s) for user management.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (2)

Event-driven and webhook contracts.

- [ClickHouse Kafka Table Engine (Consumer-Side Streaming)](https://apis.io/asyncapis/clickhouse/clickhouse-kafka-engine-asyncapi/)
- [Clickhouse Webhooks](https://apis.io/asyncapis/clickhouse/clickhouse-webhooks/)

#### Event channels (1)

Individual events and webhooks the provider emits.

- [{kafka_topic}](https://apis.io/channels/clickhouse/kafka-topic/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [clickhouse-mcp.yml](https://apis.io/servers/clickhouse/clickhouse-mcp-yml/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Clickhouse Agentic Access](https://apis.io/agentic-access/clickhouse/clickhouse-agentic-access/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Clickhouse Context](https://apis.io/jsonld/clickhouse/clickhouse-context/)

#### Collections (9)

Postman and Open Collection request collections.

- [ClickHouse HTTP Interface](https://apis.io/collections/clickhouse/open-clickhouse/)
- [ClickHouse HTTP Interface API](https://apis.io/collections/clickhouse/open-clickhouse-clickhouse-http-interface-api/)
- [ClickHouse HTTP Interface Ping API](https://apis.io/collections/clickhouse/open-clickhouse-ping-api/)
- [ClickHouse HTTP Interface Play API](https://apis.io/collections/clickhouse/open-clickhouse-play-api/)
- [ClickHouse HTTP Interface Replicas Status API](https://apis.io/collections/clickhouse/open-clickhouse-replicas-status-api/)
- [ClickHouse HTTP Interface API](https://apis.io/collections/clickhouse/postman-clickhouse-clickhouse-http-interface-api/)
- [ClickHouse HTTP Interface Ping API](https://apis.io/collections/clickhouse/postman-clickhouse-ping-api/)
- [ClickHouse HTTP Interface Play API](https://apis.io/collections/clickhouse/postman-clickhouse-play-api/)
- [ClickHouse HTTP Interface Replicas Status API](https://apis.io/collections/clickhouse/postman-clickhouse-replicas-status-api/)

#### Overlays (17)

OpenAPI overlays, including conversational phrasing for each operation.

- [Clickhouse Api Keys Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-api-keys-api-phrasing-overlay/)
- [Clickhouse Backup Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-backup-api-phrasing-overlay/)
- [Clickhouse Billing Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-billing-api-phrasing-overlay/)
- [Clickhouse Clickhouse Http Interface Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-clickhouse-http-interface-api-phrasing-overlay/)
- [Clickhouse Clickpipes Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-clickpipes-api-phrasing-overlay/)
- [Clickhouse Clickstack Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-clickstack-api-phrasing-overlay/)
- [Clickhouse Cloud Api Overlay](https://apis.io/overlays/clickhouse/clickhouse-cloud-api-overlay/)
- [Clickhouse Organization Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-organization-api-phrasing-overlay/)
- [Clickhouse Ping Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-ping-api-phrasing-overlay/)
- [Clickhouse Play Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-play-api-phrasing-overlay/)
- [Clickhouse Postgres Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-postgres-api-phrasing-overlay/)
- [Clickhouse Prometheus Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-prometheus-api-phrasing-overlay/)
- [Clickhouse Replicas Status Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-replicas-status-api-phrasing-overlay/)
- [Clickhouse Role Management Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-role-management-api-phrasing-overlay/)
- [Clickhouse Service Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-service-api-phrasing-overlay/)
- [Clickhouse Udf Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-udf-api-phrasing-overlay/)
- [Clickhouse User Management Api Phrasing Overlay](https://apis.io/overlays/clickhouse/clickhouse-user-management-api-phrasing-overlay/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [ClickHouse — asyncapi rules](https://apis.io/rules/clickhouse/clickhouse-asyncapi-spectral-rules/)
- [ClickHouse API Rules](https://apis.io/rules/clickhouse/clickhouse-rules/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Clickhouse Authentication](https://apis.io/security/clickhouse/clickhouse-authentication/)
- [Clickhouse Domain Security](https://apis.io/security/clickhouse/clickhouse-domain-security/)
- [Clickhouse Trust Center](https://apis.io/security/clickhouse/clickhouse-trust-center/)
- [Clickhouse Vulnerability Disclosure](https://apis.io/security/clickhouse/clickhouse-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Clickhouse Scopes](https://apis.io/scopes/clickhouse/clickhouse-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Clickhouse Plans Pricing](https://apis.io/plans/clickhouse/clickhouse-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Clickhouse Rate Limits](https://apis.io/rate-limits/clickhouse/clickhouse-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Clickhouse Finops](https://apis.io/finops/clickhouse/clickhouse-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://clickhouse.com/)
- [Documentation](https://clickhouse.com/docs)
- [Getting started](https://clickhouse.com/docs/quick-start)
- [API reference](https://clickhouse.com/docs/products/cloud/api-reference/organization/get-list-of-available-organizations)
- [Pricing](https://clickhouse.com/pricing)
- [Sign up](https://console.clickhouse.cloud/signUp)
- [Support](https://clickhouse.com/support)
- [Blog](https://clickhouse.com/blog)
- [Terms of service](https://clickhouse.com/legal/clickhouse-general-terms-and-conditions)
- [Privacy policy](https://clickhouse.com/legal/privacy-policy)
- [GitHub](https://github.com/ClickHouse)
- [Status](https://status.clickhouse.com/)

## API Evangelist rating

**Kin Score 72.0** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 66.7 |
| Contract quality | 61.7 |
| Contract governance | 15.9 |
| Operational transparency | 73.7 |
| Developer ergonomics | 83.3 |
| Access clarity | 78.9 |

**Agent readiness 58.4** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | verified |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | yes |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 45.1** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/clickhouse/](https://apis.io/providers/clickhouse/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for ClickHouse: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/clickhouse/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
