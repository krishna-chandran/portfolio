---
kind: work
title: "Krishna joins ThorDrive as estimation and tracking engineer"
date: 2021-10-01
dek: "FLIR, lidar, five cameras, YOLO v4 — and an airport tractor that had to name what moved."
kicker: "Work"
dateline: "Cincinnati"
event: true
categories: ["Physical AI"]
---

CINCINNATI — In October 2021 Krishnakumar Chandran joined ThorDrive as an estimation and tracking engineer. The company was building retrofits to turn airport trucks into autonomous tractors for baggage work. The appointment ran through March 2023. It was one job. The work split into two stories: this one, on perception, and the data platform that followed.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9, daylight apron: an autonomous tractor near a parked airliner, lidar and cameras on a bar, documentary, no invented branding." caption="The tractor had to share the pavement with machines and people that move." credit="Staff" />}}

This was his first long season in physical AI, after five years of enterprise AIOps and a master’s in dynamics and controls. Aircraft, ground equipment, handlers and crew do not stay still. The existing perception algorithms were not robust enough to estimate that motion in time. A miss on an apron is not a retry. It is a safety problem.

The inherited system used an extended Kalman filter on two sensors. Lidar point clouds went through DBSCAN to find objects. Camera frames went through a YOLO detector. The two streams were fused into a list of probable dynamic obstacles, each with a confidence the estimator had to believe or discard.

He redesigned the tracker for the case the airport actually has: the tractor moving and the obstacle moving, so the useful quantity is relative motion. He put motion models on the objects — equations of motion and the practical limit on how fast a pedestrian or a tug can travel — and let the filter predict and update position and velocity over time. Each object kept a unique identifier across sensor cycles so the planner was not handed a new stranger every frame. The estimator also decided whether an object was still in view, and stopped inventing it when it was not.

The rest of the stack had to feed that filter. He wrote a FLIR thermal grabber as a ROS node so heat could join the topics when light would not. He built lidar segmentation and a lidar tracker, followed the papers on ground segmentation, and pushed PointPillar and mmdetection3d for 3D detection. YOLO v4 was trained and deployed for pedestrians, cones, K-loaders and airplanes. Five RGB cameras and two lidars were fused into one geometry. C++, Python, ROS, OpenCV and PyTorch were the shop languages.

Tests and data collection ran with the airport’s team at Cincinnati/Northern Kentucky International — in these years, not earlier. The planner received a live list of obstacles with position and velocity, and used it to keep going, change path, or stop. False positives fell. Estimates tightened. Safer decisions followed.

The data infrastructure that made the R&D loop a query instead of a person on the apron is the next column.

{{< well kind="inline" prompt="Mug, 4:5: thermal still of a person and a cone on tarmac, false-color, no overlay text." caption="Heat as a topic. The grabber published frames so the estimator had another witness." credit="Staff" />}}
