---
title: "What is direct I/O, and why does ClickHouse Managed Postgres use it for backups?"
url: "https://clickhouse.com/blog/direct-io-managed-postgres-backups"
date: "2026-10-02"
feed_url: "https://clickhouse.com/rss.xml"
---
ClickHouse Managed Postgres uses direct I/O and stripe-sized reads to keep backups fast while protecting the page cache and query latency.
