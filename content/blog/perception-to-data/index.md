---
title: "What perception work teaches a data engineer"
date: 2026-08-05
dek: "If the calibration is wrong, nothing downstream is clever. Pipelines obey the same law."
kicker: "Dispatch"
dateline: "Cincinnati"
categories: ["Dispatch"]
---

Before the pipelines, there were point clouds. Segmentation that failed on an airplane. A tracker that would not settle. Five cameras and two lidars that only agreed after someone sat with the extrinsics.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a lidar point cloud of an airliner on an apron, false color, no UI chrome, documentary render." caption="An airplane is a large object. The segmenter has to admit that." src="images/wells/well-lidar-airplane.png" />}}

That work is fussy, and it is honest. If the calibration is wrong, nothing downstream is clever. The same is true of a telemetry stream: clocks, units, drops, the silent sensor.

I still prefer a system that admits what it does not know. A farm machine and an airport tractor are different beasts. The discipline of checking the input is not. That is the habit I would take to a workplace where people, models and robots already share the line.
