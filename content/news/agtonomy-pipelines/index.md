---
title: "Three pipes from the tractor: telemetry, value, and every stop"
date: 2024-06-01
dek: "C++, Vector, gRPC and a set of AWS stores — plus the migrations when the warehouse changed."
kicker: "Physical AI"
dateline: "South San Francisco"
event: true
categories: ["Physical AI"]
---

SOUTH SAN FRANCISCO — From March through June 2024 Krishnakumar Chandran designed and implemented the vehicle-to-cloud telemetry path for Agtonomy’s autonomous tractors. There had been no proper end-to-end infrastructure. Engineers needed the stream to watch algorithms under weather, soil and crop. Growers needed numbers that looked like return.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: three faint pipeline diagrams over a tractor-in-field still, documentary, no customer data." caption="Telemetry, metrics, interrupts. One agent on the machine; the autonomy stack was not to notice." credit="Staff" />}}

**Telemetry.** A custom C++ application on the tractor published high-frequency state. Vector shipped it. AWS Kinesis, S3, Timestream and OpenSearch sat on the far side, with ClickHouse and InfluxDB for analytics and series. gRPC, Protobuf, sockets and REST kept the distributed pieces honest. A vehicle-state agent wrote snapshots to Redis so live observability was not a batch job.

**Metrics.** Acres, fuel, productivity — autonomous and manual — landed where a warehouse or a lake could answer a business question. This pipe is how a grower is asked to believe the ROI argument.

**Interrupts.** Every stop for a fault, a constraint or the weather, stored so the next season is not a rumor.

**How it was run.** He researched the tools, chose the stack, and designed for high availability. Vector ran on AWS Fargate and ECS with autoscaling; ELK watched the shippers. When the store had to change, he wrote the ETL: InfluxDB to Timestream, InfluxDB to S3, S3 to ClickHouse, in batch. Docker and GitHub CI/CD carried the images. The design target was hundreds of vehicles at once, without touching core autonomy.

Bobcat and Kubota came onto the same bones. Series B sat in the same season. Growers were shown a number, not a promise.

{{< well kind="inline" prompt="Inline, 4:3: a schema sketch and a Grafana panel, no real tenant names." caption="Table design is part of the product. The farmer never sees the warehouse." credit="Staff" />}}
