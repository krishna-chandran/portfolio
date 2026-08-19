---
kind: work
title: "Three pipes from the tractor: telemetry, value, and every stop"
date: 2024-06-01
dek: "C++, Vector, gRPC and a set of AWS stores — plus the migrations when the warehouse changed."
kicker: "Work"
dateline: "South San Francisco"
event: true
categories: ["Physical AI"]
---

SOUTH SAN FRANCISCO — From March through June 2024 Krishnakumar Chandran designed and implemented the vehicle-to-cloud path for Agtonomy’s autonomous tractors. There had been no proper end-to-end infrastructure. The machines were already in the field. Engineers needed a near-real-time stream to watch algorithms under weather, soil and crop. Growers needed numbers that looked like return. The R&D loop had nowhere honest to put the tape.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: three faint pipeline diagrams over a tractor-in-field still, documentary, no customer data." caption="Telemetry, metrics, interrupts. One agent on the machine; the autonomy stack was not to notice." credit="Staff" />}}

He sat the problem first: what had to leave the tractor, how often, and what must never slow the autonomy stack. He compared architectures and data tools, chose a stack that mixed open systems with AWS, drew the end-to-end design, took the approvals, then built and tested the pipes himself. Stakeholders checked data quality and reliability before anyone called the path done.

**Telemetry.** A lightweight C++ agent on the tractor published high-frequency sensor and operational state. Vector shipped it. AWS Kinesis, S3, Timestream and OpenSearch sat on the far side, with ClickHouse and InfluxDB for analytics and series. gRPC, Protobuf, sockets and REST kept the distributed pieces honest. A vehicle-state agent wrote snapshots to Redis so live observability was not a batch job. The design target was hundreds of vehicles at once — as many as 300 talking at the same time — without touching core autonomy, and without a bill that grew faster than the fleet.

**Metrics.** The second pipe aggregated what a grower actually buys: acres covered, fuel, productivity, autonomous against manual. That is the ROI argument in a table. He designed schemas and queries so Grafana and the customer-facing boards could answer a business question without a warehouse tour. Stream processing pulled those numbers from terabytes of raw telemetry rather than asking an engineer to hunt a bag.

**Interrupts.** The third pipe recorded every stop — a fault, a constraint, the weather — so autonomy performance was not a rumor and the next season had a file. InfluxDB held the series; ClickHouse held the analytical load. He also trimmed what left the stack: less bandwidth, more signal.

When the store had to change, he wrote the migrations: InfluxDB to Timestream, InfluxDB to S3, S3 to ClickHouse, with custom ETL for batch work. Vector ran on AWS Fargate and ECS with autoscaling; ELK watched the shippers. Docker and GitHub CI/CD carried the images. Backend APIs sat where an application needed a number, not a log dump.

Bobcat and Kubota came onto the same bones. Series B sat in the same season. The path was how new OEMs could be onboarded without a second architecture, and how a grower was shown a number instead of a promise.

{{< well kind="inline" prompt="Inline, 4:3: a schema sketch and a Grafana panel, no real tenant names." caption="Table design is part of the product. The farmer never sees the warehouse." credit="Staff" />}}
