# ClickHouse (clickhouse)

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

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Analytics
- Cloud Database
- Column-Oriented
- Database
- OLAP
- Open Source
- Real-Time
- SQL

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-04-26

## APIs

### ClickHouse HTTP Interface

HTTP interface (default port 8123, HTTPS 8443) for executing SQL queries against ClickHouse. Supports SELECT via GET, mutations via POST, multiple output formats (JSON, CSV, XML, TabSeparated), and authentication via HTTP Basic, URL parameters, or X-ClickHouse-User/X-ClickHouse-Key headers. Helper paths include /ping and /replicas_status.

- **Human URL:** [https://clickhouse.com/docs/en/interfaces/http](https://clickhouse.com/docs/en/interfaces/http)
- **Base URL:** `http://localhost:8123`

#### Tags

- Database
- HTTP
- SQL

#### Properties

- [Documentation](https://clickhouse.com/docs/en/interfaces/http)
- [Postman Collection](collections/clickhouse.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clickhouse.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ClickHouse Cloud API

OpenAPI 3.1-described REST API for managing ClickHouse Cloud organizations, services, API keys, members, backups, private endpoints, and ClickHouse settings. Endpoints under /v1 with consistent envelope responses (status, requestId, result, error) and authentication via API key.

- **Human URL:** [https://clickhouse.com/docs/en/cloud/manage/api/api-overview](https://clickhouse.com/docs/en/cloud/manage/api/api-overview)
- **Base URL:** `https://api.clickhouse.cloud`

#### Tags

- Cloud
- Management
- REST

#### Properties

- [Documentation](https://clickhouse.com/docs/en/cloud/manage/api/api-overview)
- [Swagger](https://clickhouse.com/docs/cloud/manage/api/swagger)
- [OpenAPI](https://api.clickhouse.cloud/v1) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/clickhouse.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clickhouse.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ClickHouse Native TCP Interface

Native binary TCP protocol used by ClickHouse client libraries for maximum throughput between client and server (default port 9000).

- **Human URL:** [https://clickhouse.com/docs/en/interfaces/tcp](https://clickhouse.com/docs/en/interfaces/tcp)

#### Tags

- Native
- TCP

#### Properties

- [Documentation](https://clickhouse.com/docs/en/interfaces/tcp)
- [Postman Collection](collections/clickhouse.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clickhouse.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ClickHouse MySQL Interface

MySQL wire protocol compatibility allowing existing MySQL clients and BI tools to query ClickHouse without driver changes.

- **Human URL:** [https://clickhouse.com/docs/en/interfaces/mysql](https://clickhouse.com/docs/en/interfaces/mysql)

#### Tags

- MySQL
- Wire Protocol

#### Properties

- [Documentation](https://clickhouse.com/docs/en/interfaces/mysql)
- [Postman Collection](collections/clickhouse.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clickhouse.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ClickHouse PostgreSQL Interface

PostgreSQL wire protocol compatibility for connecting psql, JDBC and other PostgreSQL clients to ClickHouse.

- **Human URL:** [https://clickhouse.com/docs/en/interfaces/postgresql](https://clickhouse.com/docs/en/interfaces/postgresql)

#### Tags

- PostgreSQL
- Wire Protocol

#### Properties

- [Documentation](https://clickhouse.com/docs/en/interfaces/postgresql)
- [Postman Collection](collections/clickhouse.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clickhouse.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ClickHouse gRPC Interface

gRPC interface defined by clickhouse_grpc.proto for efficient binary communication.

- **Human URL:** [https://clickhouse.com/docs/en/interfaces/grpc](https://clickhouse.com/docs/en/interfaces/grpc)

#### Tags

- gRPC
- Protocol Buffers

#### Properties

- [Documentation](https://clickhouse.com/docs/en/interfaces/grpc)
- [Protocol  Buffers](https://github.com/ClickHouse/ClickHouse/blob/master/src/Server/grpc_protos/clickhouse_grpc.proto)
- [Postman Collection](collections/clickhouse.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clickhouse.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/clickhouseinc)
- [Website](https://clickhouse.com/)
- [Documentation](https://clickhouse.com/docs)
- [Getting Started](https://clickhouse.com/docs/en/getting-started)
- [Git Hub](https://github.com/ClickHouse/ClickHouse)
- [Blog](https://clickhouse.com/blog)
- [Community](https://clickhouse.com/community)
- [Slack](https://clickhouse.com/slack)
- [Pricing](https://clickhouse.com/pricing)
- [Support](https://clickhouse.com/support)
- [Status Page](https://status.clickhouse.com/)
- [Privacy Policy](https://clickhouse.com/legal/privacy-policy)
- [Terms of Service](https://clickhouse.com/legal/terms-of-service)
- [JSON-LD](json-ld/clickhouse-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/clickhouse-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)
- [Integrations](https://clickhouse.com/integrations)

## Maintainers

**FN:** Kin Lane
**Email:** kinlane@gmail.com
