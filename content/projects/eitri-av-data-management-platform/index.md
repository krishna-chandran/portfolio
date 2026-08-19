---
title: "Eitri, a platform for every bag a tractor records"
date: 2022-06-01
dek: "Petabytes of ROS bags, 250 times the capacity, search through clip — workflow time down 91.4 percent."
kicker: "Data"
dateline: "Cincinnati"
tags: ['c++','python','postgres','ros','elasticsearch','kibana','logstash','beats','foxglove','webviz','html','css','javascript','react.js','typescript']
categories: ["Robotics","Data science","Information Technology"]
---

CINCINNATI — Eitri was the name on an end-to-end robotics data platform built at ThorDrive: collect and store petabytes of ROS bags, live telemetry and operator logs, and hand a clip to perception. Capacity rose by about 250 times.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a dark operations UI with a map of runs, bag list, and a video-lidar scrubber, no customer data." caption="Eitri. Collect, store, find, clip, download." credit="Staff" />}}

The stack mixed the shop’s usual languages — C++, Python, Postgres, ROS — with Elasticsearch, Kibana, Logstash and Beats, plus Foxglove and Webviz for looking at the tape, and a React interface on top.

Search, visualization, snapshot, parse, label, query, clip and download cut data-workflow time by 91.4 percent. A separate ELK path against the vehicle computers cut crashes by 90 percent. This page is that product.

{{< well kind="inline" prompt="Inline, 4:3: a clip being cut from a lidar replay, yellow in and out points." caption="The cut. That is the feature." credit="Staff" />}}
