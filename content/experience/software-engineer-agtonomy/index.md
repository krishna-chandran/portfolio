---
kind: work
title: "Krishna joins Agtonomy to make a farm fleet report what the field did"
date: 2024-03-12
dek: "Software engineer, data analytics: C++, Vector, gRPC, Redis snapshots, and the ETL when the warehouse moved."
kicker: "Work"
dateline: "South San Francisco"
tags: ["c++","docker","aws","python","vector","influxdb","clickhouse","grafana","timestream","kinesis","opensearch","grpc","protobuf"]
categories: ['Robotics','Physical AI','Agtech']
---

SOUTH SAN FRANCISCO — On 12 March 2024 Krishnakumar Chandran joined Agtonomy as a software engineer in data analytics. He has since left that role. The brief was to get telemetry off autonomous farm machines and into a cloud engineers and growers could use — watch the stack, and show a number that looked like return.
<!--more-->

{{< well kind="lead" prompt="Dusk, wide, 16:9: an autonomous tractor on a vineyard row, dust in the headlights, no people, documentary still." caption="Bobcat and Kubota machines in permanent crops — if the data arrives." src="images/wells/well-tractor-vineyard.png" />}}

On the vehicle he wrote custom C++ applications, Docker images, and a real-time state agent that published snapshots to Redis. In the cloud he designed vehicle-to-cloud telemetry on Vector, InfluxDB, Timestream, OpenSearch, S3, ClickHouse and Kinesis, talking over gRPC, Protobuf, sockets and REST. Time series landed in databases, warehouses and lakes for live boards, long-term storage and business-intelligence analytics. Stream processing pulled metrics from terabytes of raw telemetry. Backend APIs fed the applications a grower or an engineer opened.

Vector ran on AWS Fargate and ECS with autoscaling and ELK monitoring. When the store changed he wrote the ETL: InfluxDB to Timestream, InfluxDB to S3, S3 to ClickHouse. Three pipes had to exist — telemetry, customer-value metrics, interrupts. The architecture was drawn for as many as 300 vehicles. On the record he played a key part in taking a fleet on the order of twenty machines toward 250, across Bobcat AT and CT and the Kubota M5N, in vineyards and olives, for mowing, spraying and scientific collection. Series B, a Kubota partnership, CES 2025, FIRA 2025 and CES 2026 sat in the same season.
