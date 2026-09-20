---
title: "Replica-aware routing public beta"
url: "https://clickhouse.com/blog/replica-aware-routing-public-beta"
date: "2026-09-15"
feed_url: "https://clickhouse.com/rss.xml"
---
Temporary tables and named sessions live on a single ClickHouse replica, so a follow-up query routed elsewhere can't see them. Replica-aware routing pins your requests to the same replica over HTTP or the native protocol — and here's how we built it.
