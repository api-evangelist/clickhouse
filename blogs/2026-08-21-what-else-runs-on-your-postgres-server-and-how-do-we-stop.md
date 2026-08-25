---
title: "What else runs on your Postgres server, and how do we stop it from taking the database down?"
url: "https://clickhouse.com/blog/protect-postgres-from-supporting-processes"
date: "2026-08-21"
feed_url: "https://clickhouse.com/rss.xml"
---
ClickHouse Managed Postgres uses runtime budgets, cgroup limits, and disk-full session exemptions to keep supporting services from compromising database availability.
