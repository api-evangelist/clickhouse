# ClickHouse (clickhouse)

ClickHouse is a fast open-source column-oriented database management system that enables real-time analytical reporting using SQL. ClickHouse exposes multiple interfaces (HTTP, native TCP, MySQL/PostgreSQL wire protocols, gRPC) and the ClickHouse Cloud management plane offers a public OpenAPI-described REST API for provisioning services, organizations, members, API keys, backups, and private endpoints.

**APIs.json:** [apis.yml](https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **x-type:** opensource

## Tags

Analytics, Cloud Database, Column-Oriented, Database, OLAP, Open Source, Real-Time, SQL

## APIs

### ClickHouse HTTP Interface
HTTP interface (port 8123 / HTTPS 8443) for executing SQL queries. SELECT via GET, mutations via POST, multiple output formats and authentication via HTTP Basic, URL parameters, or `X-ClickHouse-User`/`X-ClickHouse-Key` headers.

- [Documentation](https://clickhouse.com/docs/en/interfaces/http)

### ClickHouse Cloud API
OpenAPI 3.1-described REST API for managing ClickHouse Cloud organizations, services, API keys, members, backups, private endpoints, and ClickHouse settings.

- [Documentation](https://clickhouse.com/docs/en/cloud/manage/api/api-overview)
- [Swagger](https://clickhouse.com/docs/cloud/manage/api/swagger)
- [OpenAPI](https://api.clickhouse.cloud/v1)

### ClickHouse Native TCP Interface
Native binary TCP protocol used by ClickHouse client libraries for maximum throughput (port 9000).

- [Documentation](https://clickhouse.com/docs/en/interfaces/tcp)

### ClickHouse MySQL Interface
MySQL wire protocol compatibility for existing MySQL clients and BI tools.

- [Documentation](https://clickhouse.com/docs/en/interfaces/mysql)

### ClickHouse PostgreSQL Interface
PostgreSQL wire protocol compatibility for psql, JDBC and other PostgreSQL clients.

- [Documentation](https://clickhouse.com/docs/en/interfaces/postgresql)

### ClickHouse gRPC Interface
gRPC interface defined by `clickhouse_grpc.proto` for efficient binary communication.

- [Documentation](https://clickhouse.com/docs/en/interfaces/grpc)
- [Protocol Buffers](https://github.com/ClickHouse/ClickHouse/blob/master/src/Server/grpc_protos/clickhouse_grpc.proto)

## Common Properties

- [Website](https://clickhouse.com/)
- [Documentation](https://clickhouse.com/docs)
- [GitHub](https://github.com/ClickHouse/ClickHouse)
- [Slack](https://clickhouse.com/slack)
- [Status](https://status.clickhouse.com/)
- [JSON-LD](json-ld/clickhouse-context.jsonld)
- [Spectral](rules/clickhouse-rules.yml)
- [Naftiko Capabilities](capabilities/clickhouse-capabilities.yml)

## Maintainers

- **FN:** Kin Lane
- **Email:** kinlane@gmail.com
