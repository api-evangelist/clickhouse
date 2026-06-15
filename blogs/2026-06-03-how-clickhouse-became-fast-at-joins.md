---
title: "How ClickHouse became fast at joins"
url: "https://clickhouse.com/blog/clickhouse-fast-joins"
date: "2026-06-03"
author: "Tom Schreiber"
feed_url: "https://clickhouse.com/blog"
---
Over two years of engineering focused on join optimization, ClickHouse achieved a 26x performance improvement on the TPC-H SF100 join-heavy workload. The improvements involved implementing parallel hash joins, runtime filters, lazy column replication, and statistics-based join reordering to make joins competitive by default.
