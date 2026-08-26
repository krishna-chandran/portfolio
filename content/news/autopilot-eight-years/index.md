---
kind: opinion
title: "Eight years on, Krishna flies the Cincinnati autopilot again — this time in a browser"
date: 2026-08-26
dek: "A Fall 2017 class assignment leaves MATLAB. Friends and connections can take the stick without a lab license."
kicker: "Opinion"
dateline: "Los Angeles"
event: true
image: "images/wells/well-uav-browser.png"
categories: ["Aerospace"]
---

LOS ANGELES — Krishnakumar Chandran, MEngg Aerospace, sat again with a file from Fall 2017: Unmanned Aerial Systems, Chapter 5 Autopilot, University of Cincinnati, under Prof. Dr. Rajnikanth Sharma, with Dr. Anusna Chakraborty as teaching assistant. Eight years later the same small airplane is not a MATLAB session. It is a page. He put it there, with help from AI, so friends and connections could fly it without the lab.
<!--more-->

The original brief was a class, not a product. A small fixed-wing would hold its speed, its height and its heading, and it would do that over a world you could watch. The work lived in MATLAB. Classmates needed the toolbox. Visitors needed an account. The memory stayed on a drive.

This year he opened that drive. The loops are the same idea — keep the numbers you asked for — but the room is a browser. No install. A link is enough. [linkedin.com/in/krish-na](https://linkedin.com/in/krish-na) is on the title card for anyone who wants the rest of the paper.

## What you are looking at

The airplane is Krishna's UAV, with the book Aerosonde as a second skin. It flies a toy Cincinnati: suburbs on a grid, a downtown of towers, a lake, ridges to the west. A radio line at the bottom greets you, gives the weather, then says what the airplane is trying to do and what ground is under the wing.

The panel on the right is the scoreboard. The names are the ordinary language of that course, written short:

- **Airspeed (Va)** — how fast the air is coming at the nose, in meters a second. The number after the slash is what you asked for.
- **Altitude (h)** — height above the ground, in meters.
- **Course (χ)** — the path over the ground, in degrees from north.
- **Roll, pitch, yaw (φ, θ, ψ)** — bank, nose up or down, and which way the nose is pointed.
- **North, East** — where it is on the map.
- **Elevator, aileron, rudder, throttle (δe, δa, δr, δt)** — the moving bits. Gold surfaces blush cyan or rose when they move.

## How to enjoy it

Open the [class write-up]({{< relref "projects/autopilot-fixedwing-uav" >}}) or go straight to the [full-page sim](/portfolio/sims/uav-autopilot/).

W and S, or the up and down arrows, raise and lower the altitude you want. A and D, or left and right, change course. Space pauses. Three sliders at the bottom do the same work if you would rather drag. The dashed line on the minimap is the course you asked for; the wedge is the course she has. The subtitle types a greeting first, then the loops, then the landscape — suburbs, downtown, the lake — and what she is heading toward.

Minimize the right-hand card if you want more sky. On a phone the title card hides itself so the airplane keeps the screen.

{{< sim src="sims/uav-autopilot/" title="Fixed-wing Chapter 5 autopilot" >}}

He is not claiming the class is finished. He is claiming it can be shared. Eight years is long enough for a MATLAB file to go quiet. A link is a way to hear it again.
