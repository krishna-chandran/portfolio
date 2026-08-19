---
title: "Krishna joins Agtonomy to make a farm fleet report what the field did"
date: 2024-03-12
dek: "Software engineer, data analytics: a C++ agent, Vector, gRPC, and vehicle-to-cloud pipes that have to stay up."
kicker: "Appointment"
dateline: "South San Francisco"
event: true
categories: ["Physical AI"]
---

SOUTH SAN FRANCISCO — On 12 March 2024 Krishnakumar Chandran joined Agtonomy as a software engineer in data analytics. The title on the card is still current. Agtonomy builds autonomy for agricultural machines — Bobcat and Kubota among the OEMs. The brief was to get telemetry off the tractor and into a cloud that engineers and growers could actually use.
<!--more-->

{{< well kind="lead" prompt="Dusk, wide, 16:9: an autonomous tractor on a vineyard row, dust in the headlights, no people, documentary still." caption="Permanent crops. Mowing, spraying and scientific collection — if the data arrives." credit="Staff" />}}

Labor is short and the row is long. A tractor that cannot report is only half a robot.

**The duties.** Write the vehicle-side software and the cloud path. Build custom C++ applications, Docker images, and pipelines on Vector, InfluxDB, AWS Timestream, AWS OpenSearch, AWS S3, ClickHouse and AWS Kinesis. Keep distributed systems talking over gRPC, Protobuf, sockets and REST. Own a real-time vehicle-state agent that publishes snapshots to Redis. Research the data tools on the market and pick what fits each need. Design vehicle-to-cloud telemetry that is scalable, flexible and highly available. Land time-series data in databases, warehouses and lakes — real-time observability, long-term storage, and business-intelligence analytics. Run Vector on AWS Fargate and ECS with autoscaling and ELK monitoring. Move data between systems when the store changes: InfluxDB to Timestream, InfluxDB to S3, S3 to ClickHouse, with custom ETL for batch work.

**How it was done.** Three pipes had to exist: telemetry, customer metrics, and interrupts. The agent on the tractor was kept light so the autonomy stack would not notice. The architecture was drawn for as many as 300 vehicles at once. He played a key part in taking a fleet that had been on the order of twenty machines toward 250, across OEMs.

Grafana and Kibana were the boards; Metabase sat where a business question needed a SQL answer. During this period the company closed a Series B, took a partnership with Kubota, automated Bobcat AT and CT machines and the Kubota M5N, and put the work on a stage at CES and FIRA. The next column is the pipeline season in detail.

{{< well kind="inline" prompt="Close, 4:3: Grafana-style board of fleet metrics, acres and stops, no customer names, documentary." caption="Throughput and stops. That is how a grower is asked to believe in physical AI." credit="Staff" />}}
