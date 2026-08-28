---
kind: work
title: "At ThorDrive, one engineer builds the platform that takes in the tractor’s tape"
seo_title: "ROS bag data platform for airport tractors · Krishna Chandran"
date: 2022-03-01
dek: "Petabytes of ROS bags, a 250-times jump in capacity, and a workflow that ran 91.4 percent faster."
image_alt: "Airport tractor data desk: ROS bags, search, clip and download"
kicker: "Work"
dateline: "Cincinnati"
event: true
categories: ["Physical AI"]
---

CINCINNATI — While he held the estimation-and-tracking card at ThorDrive, Krishnakumar Chandran also designed the company’s internal big-data platform. Autonomous tractors were producing ROS bags, live telemetry and operator logs faster than the shop could keep them. Field testing still meant a person on the apron. He built the place those files went, and the path that let an engineer troubleshoot a vehicle from the cloud.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9, night shop: an airport tractor under work lights, lidar spinning, a laptop on the fender, documentary." caption="Field testing used to mean a person on the apron. The platform tried to make it a query." src="images/wells/well-night-shop-tractor.png" />}}

The perception work needed tape. The tape had nowhere honest to live. He took the data job end to end — the career file says he built the infrastructure himself — so perception could train, debug and clip without waiting on a drive in a bag.

The platform later called Eitri collected and stored petabytes of ROS bags, live vehicle telemetry and operator logs, and raised data capacity by about 250 times. On top of that store he built the features a robotics shop actually uses: search, visualization, snapshot, parse, label, query, clip and download. Data-workflow time improved by 91.4 percent. A clip stopped being a week of archaeology.

The stack sat on AWS — S3 and EC2 — with Elasticsearch, Logstash, Kibana and Beats for the hunt, Postgres underneath, Foxglove and Webviz for looking at the tape, and a React interface on top. A separate ELK path against the vehicle computers cut crashes by 90 percent, on the record he filed. That path is how a fault became a board instead of a tow.

The same principles he had used on ignio — reliability, scalability, observability — had to hold for a ROS bag, not only for a ServiceNow queue. Combining AIOps habits with ROS, dynamics and controls, and big-data pipelines is what made the R&D loop remote. Developer workflow improved; the shop could use robotics data to write autonomy algorithms without standing next to the machine. Productivity, on that file, rose by more than 90 percent.

Once the tractor left the lot, the data path was the product.

{{< well kind="inline" prompt="Overhead, 4:3: a ROS bag timeline, yellow clips, dark UI, no faces." caption="Find the clip. That is the whole product." src="images/wells/well-ros-timeline.png" />}}
