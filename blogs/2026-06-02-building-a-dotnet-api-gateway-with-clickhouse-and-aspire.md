---
title: "Building a .NET API Gateway with ClickHouse and Aspire"
url: "https://clickhouse.com/blog/dotnet-api-gateway-aspire"
date: "2026-06-02"
author: "Alex Soffronow Pagonidis"
feed_url: "https://clickhouse.com/blog"
---
This tutorial demonstrates constructing a .NET API gateway using YARP and Aspire that logs every proxied request to ClickHouse for aggregate analytics. The implementation leverages a materialized view to maintain dashboard query performance as traffic volume increases, while using Aspire to orchestrate ClickHouse, backend services, and observability components.
