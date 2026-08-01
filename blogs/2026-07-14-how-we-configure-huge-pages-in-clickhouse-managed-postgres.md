---
title: "How we configure huge pages in ClickHouse Managed Postgres"
url: "https://clickhouse.com/blog/huge-pages-clickhouse-managed-postgres"
date: "2026-07-14"
feed_url: "https://clickhouse.com/rss.xml"
---
How ClickHouse Managed Postgres reserves, enforces, and sizes huge pages so shared_buffers avoids the per-connection page-table tax that eats RAM and stalls reads on 4KB pages.
