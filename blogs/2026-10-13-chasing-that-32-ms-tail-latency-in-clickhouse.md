---
title: "Chasing that 32 ms tail latency in ClickHouse"
url: "https://clickhouse.com/blog/chasing-32ms-tail-latency-clickhouse"
date: "2026-10-13"
feed_url: "https://clickhouse.com/blog/index.xml"
---
A customer saw an extra ~32 ms on simple SELECT queries after idle periods. We traced it to unbatched Native protocol metadata packets overflowing a reset TCP congestion window, reproduced it with network namespaces, and fixed it by batching them.
