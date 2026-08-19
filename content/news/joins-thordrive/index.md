---
title: "Krishna joins ThorDrive as estimation and tracking engineer"
date: 2021-10-01
dek: "FLIR, lidar, five cameras, YOLO v4 — and an airport tractor that had to name what moved."
kicker: "Appointment"
dateline: "Cincinnati"
event: true
categories: ["Physical AI"]
---

CINCINNATI — In October 2021 Krishnakumar Chandran joined ThorDrive as an estimation and tracking engineer. The company was building retrofits to turn airport trucks into autonomous tractors for baggage work. The appointment ran through March 2023. It was one job. The work split into two stories: this one, on perception, and the data platform that followed.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9, daylight apron: an autonomous tractor near a parked airliner, lidar and cameras on a bar, documentary, no invented branding." caption="The tractor had to share the pavement with machines and people that move." credit="Staff" />}}

Aircraft, ground equipment, handlers and crew do not stay still. The existing perception algorithms were not robust enough to say so in time.

**The duties.** Put a FLIR thermal camera into the perception stack as a ROS node. Build lidar segmentation, a lidar tracker, and the fusion that joined cameras to range. Follow the papers on ground segmentation. Improve PointPillar and mmdetection3d models for 3D object detection. Train and deploy YOLO v4 for pedestrians, cones, K-loaders and airplanes. Fuse five RGB cameras and two lidars. Hand planning a live list of obstacles it could trust.

**How it was done.** The inherited system used an extended Kalman filter on DBSCAN lidar and a camera read by YOLO. He redesigned the tracker for relative motion — the tractor moving, the obstacle moving — with motion models and speed limits a pedestrian or a tug would obey. Each object kept an identifier across cycles. Heat counted when light would not. Tests and data collection ran with the airport’s team at Cincinnati/Northern Kentucky International, in these years, not earlier.

C++, Python, ROS, OpenCV and PyTorch were the shop languages. Safer stops and path changes followed fewer false positives. The data infrastructure that made the loop remote is the next column.

{{< well kind="inline" prompt="Mug, 4:5: thermal still of a person and a cone on tarmac, false-color, no overlay text." caption="Heat as a topic. The grabber published frames so the estimator had another witness." credit="Staff" />}}
