---
title: "At ThorDrive, one engineer builds the platform that takes in the tractor’s tape"
date: 2022-03-01
dek: "Petabytes of ROS bags, a 250-times jump in capacity, and a workflow that ran 91.4 percent faster."
kicker: "Autonomy"
dateline: "Cincinnati"
event: true
categories: ["Physical AI"]
---

CINCINNATI — While he held the estimation-and-tracking card at ThorDrive, Krishnakumar Chandran also designed the company’s internal big-data platform. Autonomous tractors were producing ROS bags, live telemetry and operator logs faster than the shop could keep them. He built the place those files went.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9, night shop: an airport tractor under work lights, lidar spinning, a laptop on the fender, documentary." caption="Field testing used to mean a person on the apron. The platform tried to make it a query." credit="Staff" />}}

**The duties.** Collect and store petabytes of bag files, live vehicle telemetry and operator logs. Raise data capacity by about 250 times. Give perception search, visualization, snapshot, parse, label, query, clip and download, so a clip was not a week of archaeology. Architect ELK pipelines against the vehicle computers so a crash could be read in the cloud.

**How it was done.** The internal platform later called Eitri sat on AWS — S3 and EC2 — with Elasticsearch, Logstash, Kibana and Beats for the hunt, Postgres underneath, Foxglove and Webviz for the tape, and a React interface on top. Data-workflow time improved by 91.4 percent. The ELK path for troubleshooting vehicle computers cut vehicle crashes by 90 percent, on the record he filed.

This was the first long season in physical AI after five years of AIOps. The same principles — reliability, scalability, observability — had to hold for a ROS bag, not only for a ServiceNow queue. Once the tractor left the lot, the data path was the product.

{{< well kind="inline" prompt="Overhead, 4:3: a ROS bag timeline, yellow clips, dark UI, no faces." caption="Find the clip. That is the whole product." credit="Staff" />}}
