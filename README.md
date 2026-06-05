# ClickHouse (clickhouse)

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
