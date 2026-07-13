---
title: "How we scale PgBouncer in ClickHouse Managed Postgres"
url: "https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres"
date: "2026-07-01"
author: ""
feed_url: "https://clickhouse.com/rss.xml"
---
ClickHouse Managed Postgres runs a peered fleet of PgBouncer processes using so_reuseport to scale connection pooling across every CPU core.
