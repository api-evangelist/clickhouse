---
title: "A Quadrillion Rows across three Clouds: scaling LogHouse"
url: "https://clickhouse.com/blog/a-quadrillion-rows-across-the-three-cloud-scaling-loghouse"
date: "2026-06-30"
feed_url: "https://clickhouse.com/rss.xml"
---
We scaled our internal logging platform from 19 PiB to 431 PiB and 1.59 quadrillion rows. Here’s how we rearchitected LogHouse to handle 80 GiB/s of writes while keeping queries fast and the underlying complexity invisible.
