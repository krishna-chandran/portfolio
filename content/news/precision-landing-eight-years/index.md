---
kind: opinion
title: "Eight years on, Krishna lands the Cincinnati quadrotor on a truck that will not sit still"
seo_title: "Precision landing a quadrotor on a moving truck · Krishna Chandran"
date: 2026-08-28
dek: "A Fall 2017 precision-landing file leaves MATLAB. The gimbaled camera is the only sight of the pad."
image_alt: "Quadrotor precision landing on a moving yellow truck, gimbal camera locked, Cincinnati geolocation chapter"
kicker: "Opinion"
dateline: "Los Angeles"
event: true
image: "images/wells/well-quad-geo.png"
categories: ["Aerospace"]
---

LOS ANGELES — Krishnakumar Chandran, MEngg Aerospace, sat again with a file from Fall 2017: Precision Landing, University of Cincinnati, under Prof. Dr. Rajnikanth Sharma, with Dr. Anusna Chakraborty as teaching assistant. The brief was not a hover. It was a landing on a truck that kept moving. Eight years later the same quadrotor is not a MATLAB session. It is a still you can read. He put it there, with help from AI, so the class could be shown without the lab.
<!--more-->

The original assignment lived in MATLAB and Simulink. A twelve-state quadrotor, a gimbaled camera, a moving target, and a stack of loops that had to close the gap without drama. Classmates needed the toolbox. Visitors needed an account. The memory stayed on a drive.

This year he opened that drive. The loops are the same idea — find the truck, match its speed, step down onto the pad — but the room is a browser. [linkedin.com/in/krish-na](https://linkedin.com/in/krish-na) is on the title card for anyone who wants the rest of the paper.

{{< well kind="lead" prompt="Wide still from the sim: a quadrotor over Cincinnati suburbs, payload camera locked on a yellow truck, documentary screenshot crop." caption="Chapter 4, geolocation. The camera is locked. The loops are flying the estimate, not the truck’s true north and east." src="images/wells/well-quad-geo.png" />}}

## What was done

The work was four rooms, stacked.

**Attitude.** Inner-loop PD on roll, pitch and yaw, so the quadrotor could hover before anyone asked it to chase a truck.

**Trajectory.** Differential flatness mapped a position error to thrust, commanded bank and commanded pitch. An LQR gain sat on that error. The [trajectory write-up]({{< relref "projects/trajectory-navigation-quadcopter" >}}) is the same outer loop, asked to hold a path instead of a pad.

**Landing on truth.** The guidance law was given the truck’s north, east and velocity. It planned an intercept ahead of the vehicle, arrived matching its speed, then stepped altitude down as the horizontal range closed.

**Landing on geolocation.** The gimbal stayed on the truck. The camera was the only sight of the pad. Pixels became a line-of-sight; a filter turned that line into north, east and range; a second filter held the truck’s motion so the loops could chase a moving estimate, not a frozen pin.

The [class write-up]({{< relref "projects/landing-quadcopter-on-moving-ground-vehicle" >}}) is the 2017 paper of record. The MATLAB source sits at [uav-precision-landing](https://github.com/krishna-chandran/uav-precision-landing). The fixed-wing [autopilot]({{< relref "news/autopilot-eight-years" >}}) is the other Cincinnati file from the same year.

## What you are looking at

The still is Chapter 4. A yellow truck on a north–south road through a toy Cincinnati. A payload camera with a lock and a blob. A chase map. The panel on the right is the scoreboard, written short:

- **Range** — how far to the pad, in meters.
- **Truck** — how fast the ground vehicle is moving.
- **Geo error** — how far the estimate sits from the truck’s true north and east. The loops do not get that truth.
- **Thrust and torques** — the motors. Hover for this airframe is about 15.3 N.

The radio line at the bottom says the rule out loud: the gimbaled camera is the only sight of the truck.

He is not claiming the class is finished. He is claiming it can be shown. Eight years is long enough for a MATLAB file to go quiet. A still is a way to hear it again.
