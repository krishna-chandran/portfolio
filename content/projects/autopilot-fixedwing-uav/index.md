---
title: "An autopilot for a small fixed wing, twelve degrees of freedom"
date: 2017-08-20
dek: "Trim, PID loops and a state machine, flown in Gazebo under ROS, for takeoff through landing."
kicker: "Aerospace"
dateline: "Cincinnati"
tags: ['python','matlab','gazebo','ros','c++','simulink']
categories: ["Robotics","Self-driving Car"]
---

CINCINNATI — Equations of motion with twelve degrees of freedom were written for a fixed-wing UAV, inspected for stability, and wrapped in PID loops for roll, pitch, altitude, course, airspeed-with-throttle and airspeed-with-pitch, each with trim in mind.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a Gazebo still of a small fixed-wing UAV on a runway, ROS overlays faint, documentary screenshot crop." caption="Gazebo, under ROS. Elevator, aileron and throttle for takeoff, climb, cruise and landing." src="images/wells/well-gazebo-uav.png" />}}

A state machine switched flying modes. Gains were tuned. The code went into Python and C++ and was tested in Gazebo. The aim was the surface commands — elevator, aileron, throttle — for those flight conditions, not a demo reel.

The same Beard and McLain Chapter 5 loops now run in the browser — successive loop closure for airspeed, altitude and course, with Krishna's UAV and the book Aerosonde.

{{< sim src="sims/uav-autopilot/" title="Fixed-wing Chapter 5 autopilot" >}}

<iframe width="560" height="315" src="https://www.youtube.com/embed/7bexe2ZTbrM?si=N3MegxdIMFwZlY9Z" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

{{< well kind="wide" prompt="Wide still from the sim: the aircraft in a climbing turn, HUD-like traces of airspeed and altitude, no startup branding." caption="Climb. The state machine has a name for this." src="images/wells/well-uav-climb.png" />}}
