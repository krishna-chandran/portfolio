---
kind: work
title: "Krishna joins ThorDrive as estimation and tracking engineer"
date: 2021-10-01
dek: "One job, through March 2023: FLIR, five cameras, two lidars, YOLO v4, then a platform for the bags."
kicker: "Work"
dateline: "Cincinnati"
skills: ['deep-learning','computer-vision','c++','python','ros','yolov4','lidar','sensor-fusion','pointpillar','pytorch']
fields: ['Robotics','Physical AI']
---

CINCINNATI — In October 2021 Krishnakumar Chandran joined ThorDrive as an estimation and tracking engineer. The appointment ran through March 2023. It was one job. The company was retrofitting airport trucks into autonomous baggage tractors. This was the first long season in physical AI.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9, daylight apron: an autonomous tractor near a parked airliner, lidar and cameras on a bar, documentary, no invented branding." caption="CVG’s ground, in the ThorDrive years." credit="Staff" />}}

The inherited system fused DBSCAN lidar and YOLO camera detections into an extended Kalman filter. He redesigned the tracker for relative motion — tractor and obstacle both moving — with motion models and speed limits a pedestrian or a tug would obey. Each object kept an identifier across cycles. The planner received a live list of position and velocity, and used it to keep going, change path, or stop.

He wrote a FLIR grabber as a ROS node, built lidar segmentation and a lidar tracker, followed the papers on ground segmentation, pushed PointPillar and mmdetection3d, trained YOLO v4 for pedestrians, cones, K-loaders and airplanes, and fused five RGB cameras with two lidars. Tests ran at Cincinnati/Northern Kentucky International. False positives fell. The data platform built in the same appointment is a separate story.
