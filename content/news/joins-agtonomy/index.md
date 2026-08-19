---
kind: work
title: "Krishna joins Agtonomy to make a farm fleet report what the field did"
date: 2024-03-12
dek: "Software engineer, data analytics: a C++ agent, Vector, gRPC, and vehicle-to-cloud pipes that have to stay up."
kicker: "Work"
dateline: "South San Francisco"
event: true
categories: ["Physical AI"]
---

SOUTH SAN FRANCISCO — On 12 March 2024 Krishnakumar Chandran joined Agtonomy as a software engineer in data analytics. He has since left that role. Agtonomy builds autonomy for agricultural machines — Bobcat and Kubota among the OEMs — and the brief was not another dashboard. It was to get telemetry off the tractor and into a cloud that engineers and growers could actually use: watch the stack under weather, soil and crop, and show a farmer a number that looked like return.
<!--more-->

{{< well kind="lead" prompt="Dusk, wide, 16:9: an autonomous tractor on a vineyard row, dust in the headlights, no people, documentary still." caption="Permanent crops. Mowing, spraying and scientific collection — if the data arrives." credit="Staff" />}}

Labor is short and the row is long. A tractor that cannot report is only half a robot. Farming has run on the same habits for a century; physical AI is new to that field. The platforms he built were how a grower was asked to believe the machines, and how the company was asked to scale them.

The job on the card was data. The work sat on both sides of the radio. On the vehicle he wrote custom C++ applications, Docker images, and a real-time state agent that published snapshots to Redis so live observability was not a batch job. In the cloud he designed vehicle-to-cloud telemetry that had to be scalable, flexible and highly available, then landed time-series in databases, warehouses and lakes — InfluxDB, AWS Timestream, OpenSearch, S3, ClickHouse, Kinesis — for real-time boards, long-term storage and business-intelligence analytics. gRPC, Protobuf, sockets and REST kept the distributed pieces talking.

He also sat the quieter half of a data job: research the tools on the market, pick what fit each need, and own the migrations when the store changed. Vector ran on AWS Fargate and ECS with autoscaling and ELK monitoring. When InfluxDB had to give way, he wrote the ETL — InfluxDB to Timestream, InfluxDB to S3, S3 to ClickHouse — in batch. Stream processing pulled useful metrics from terabytes of raw telemetry. Backend APIs fed the applications a grower or an engineer actually opened. Grafana and Kibana were the boards; Metabase sat where a business question needed SQL.

Three pipes had to exist: high-frequency telemetry, customer-value metrics, and every interrupt that stopped a machine. The agent on the tractor was kept light so the autonomy stack would not notice. The architecture was drawn for as many as 300 vehicles at once, and for more than one OEM. On the record he played a key part in taking a fleet that had been on the order of twenty machines toward 250.

Agtonomy automated Bobcat AT and CT machines and the Kubota M5N, in vineyards and olives, for mowing, spraying and scientific collection. During this period the company closed a Series B, took a partnership with Kubota, and put the work on a stage at CES 2025, FIRA 2025 and CES 2026. The next column is the pipeline season in detail.

{{< well kind="inline" prompt="Close, 4:3: Grafana-style board of fleet metrics, acres and stops, no customer names, documentary." caption="Throughput and stops. That is how a grower is asked to believe in physical AI." credit="Staff" />}}
