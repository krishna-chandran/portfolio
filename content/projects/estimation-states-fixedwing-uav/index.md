---
title: "An EKF for a fixed wing that has to know where it is"
date: 2017-11-01
dek: "Takeoff, cruise, landing in MATLAB, then Python and C++ in Gazebo under ROS."
kicker: "Aerospace"
dateline: "Cincinnati"
tags: ['ros','matlab','simulink','linux','python','c++']
categories: ["Robotics"]
---

CINCINNATI — State estimation for an autonomous fixed-wing aircraft was written as an extended Kalman filter from the vehicle’s dynamics, then checked in MATLAB and Simulink for takeoff, cruise and landing.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: MATLAB scopes of estimated vs true states during a takeoff run, muted academic screenshot." caption="The filter, on takeoff. Gazebo came after the scopes went quiet." credit="Staff" />}}

The algorithm was implemented in Python and C++, run under ROS, and tested in Gazebo. The aim was the states themselves — not a prettier HUD.
