---
title: "Lidar segmentation, taught to see an airplane"
date: 2022-01-01
dek: "A point cloud that treats a jet as clutter is not ready for the apron."
kicker: "Perception"
dateline: "Cincinnati"
tags: ['c++','linux','ros']
categories: ["Robotics","Self-driving Car"]
---

CINCINNATI — Lidar segmentation on the airport tractor failed, at first, in a simple way: airplanes are very large. The algorithm had to be taught to cut them out of the cloud as objects, not weather.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a dense lidar cloud of a parked airplane, fuselage segmented in a second color, apron at dusk." caption="The jet, as a cluster. That was the whole assignment." src="images/wells/well-lidar-airplane.png" />}}

The work ran in C++ and ROS, following the papers on ground segmentation, and sat beside PointPillar and mmdetection3d work for 3D detection. Five RGB cameras and two lidars were fused in the same season. If the segmenter blinks, the tracker inherits a hole.
