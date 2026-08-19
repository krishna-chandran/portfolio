---
kind: work
title: "At HAL, a Tejas slat actuator is asked why it developed play"
date: 2014-01-15
dek: "After about 300 flights the mechanism moved when it should not. The work was equations, a redundant link, CATIA and ANSYS."
kicker: "Work"
dateline: "Chennai"
event: true
categories: ["Aerospace"]
---

CHENNAI — In the first months of 2014 Krishnakumar Chandran worked with Hindustan Aeronautics on the Tejas. A slat actuator — the mechanism that drives a leading-edge control surface — was developing play after about 300 operational runs. Unwanted motion damaged the parts around the lug. In that condition the aircraft was not fit to keep flying on the old geometry.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: CATIA-style actuator link, neutral gray, studio, no proprietary dimensions." caption="The redundant link. Cantilever theory first, then the mesh." src="images/wells/well-actuator-link.png" />}}

The project ran from January through April 2014, as a collaboration with HAL’s assembly line. The brief was a root cause and a fix that could be proven. If the analysis matched the case on the aircraft, and if a finite-element check in ANSYS backed the fix, the lifetime of the mechanism could be extended. Funding was none; the college project was the vehicle.

He first derived approximate equations for the existing actuator under load: geometry, material, forces and moments near the lug that was taking the damage. Cantilever-beam theory said where the concentration lived. He proposed a redundant member — a link — to spread that load, then derived the modified case by hand. The pad said the play would fall and the structure would carry the control-surface loads more evenly.

The team modeled both configurations in CATIA V5 — the existing assembly and the one with the link — and took them to ANSYS: control-surface loads, force and moment distributions, stress, strain, the operating case. The mesh agreed with the pad. HAL’s engineering team used the findings in later development and evaluation.

His part of the job was the mathematics and the argument for the link, then the CATIA assembly with the team. The paper that recorded the method, with Manikandan C and Niranjana S, ran on 1 October 2014 in the *Journal of Basic and Applied Engineering Research*.

{{< well kind="inline" prompt="Inline, 4:3: ANSYS-style stress plot, muted colors, no readable dimensions." caption="Hand calculations, then the finite-element check. HAL took the file forward." src="images/wells/well-ansys-plot.png" />}}
