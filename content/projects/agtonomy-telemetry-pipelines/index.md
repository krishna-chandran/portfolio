---
title: "Three pipes from the tractor: telemetry, value, and every stop"
date: 2024-06-01
dek: "A C++ agent, Vector, InfluxDB and ClickHouse — architecture for hundreds of machines, built in a Series B year."
kicker: "Physical AI"
dateline: "South San Francisco"
tags: ['c++','aws','vector','influxdb','clickhouse','grafana','kinesis','grpc','fargate']
categories: ["Robotics","Agtech","Physical AI"]
---

SOUTH SAN FRANCISCO — Agtonomy’s tractors needed a near-real-time path to the cloud and did not have one. From March through June 2024 the job was to design that path with open tools, then keep it as the fleet grew.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: three faint pipeline diagrams over a tractor-in-field still, documentary, no customer data." caption="Telemetry, metrics, interrupts. One agent on the machine; the autonomy stack was not to notice." credit="Staff" />}}

The first pipe was telemetry: a custom C++ application, Vector as shipper, gRPC and Protobuf on the wire, AWS Kinesis, S3, Timestream and OpenSearch on the far side, a vehicle-state agent writing snapshots to Redis. Vector ran on Fargate and ECS with autoscaling. The second pipe was metrics — acres, fuel, productivity. The third was interrupts: every stop.

When the store changed, custom ETL moved InfluxDB to Timestream, InfluxDB to S3, and S3 to ClickHouse. Grafana and Kibana were the boards. New OEMs, including Bobcat and Kubota, could be onboarded on the same bones. The company closed a Series B in the same season.
