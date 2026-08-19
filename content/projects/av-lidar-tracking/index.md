---
title: "The estimator names every moving thing on the apron"
date: 2021-10-01
dek: "DBSCAN, YOLO, an EKF and a unique ID — so the planner can stop, turn or go."
kicker: "Perception"
dateline: "Cincinnati"
tags: ['c++','linux','ros','ekf','yolo','dbscan']
categories: ["Robotics","Physical AI"]
---

CINCINNATI — ThorDrive’s airport tractor had a tracker that was not robust enough for a live apron. Aircraft, tugs, bags and people move. The tractor moves. Relative motion is the whole problem.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: lidar boxes and camera IDs on an apron, one pedestrian and a tug, muted overlay, documentary." caption="A live list: position, velocity, still in view. The planner reads it or it is decoration." credit="Staff" />}}

Lidar went through DBSCAN; the camera through YOLO; the two were fused. An extended Kalman filter, rebuilt with motion models and speed limits a pedestrian or a ground vehicle would actually keep, predicted and updated each object and kept an identifier across cycles.

The output was a real-time list for planning: continue, change path, or stop. False positives fell. The states got cleaner. Tests ran at Cincinnati/Northern Kentucky International with the airport’s team.
