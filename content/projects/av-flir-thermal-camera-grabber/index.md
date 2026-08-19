---
title: "A FLIR camera, talking ROS, so heat could join the stack"
date: 2021-10-01
dek: "A grabber node publishes thermal frames for objects that light will not always confess."
kicker: "Perception"
dateline: "Cincinnati"
tags: ['c++','linux','ros','ci-cd-pipeline']
categories: ["Robotics"]
---

CINCINNATI — The perception stack needed thermal frames as ROS topics, not as a vendor GUI. Krishnakumar Chandran wrote a FLIR grabber node so the rest of the ThorDrive tractor could subscribe.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a FLIR brick on a sensor bar, cables, tractor hood, documentary." caption="Heat as a topic. Pedestrians and hot metal do not always wait for RGB." src="images/wells/well-flir-bar.png" />}}

The aim was a data stream from the hardware to the stack, for objects that are thermally obvious even when they are visually shy.
