---
title: "Krishna joins the IMS lab to ask a Mazak spindle to confess early"
date: 2018-07-22
dek: "A full-stack engineer on a Mazak-funded project: vibration, current, a classifier, and a health score from 0 to 100."
kicker: "Appointment"
dateline: "Cincinnati"
event: true
categories: ["Industrial AI"]
---

CINCINNATI — On 22 July 2018 Krishnakumar Chandran joined the Intelligent Maintenance Systems laboratory at the University of Cincinnati as a full-stack engineer. The project was funded by Mazak Corporation. The objective was to predict CNC spindle failure before the floor hears it.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a Mazak CNC in a university lab, vibration cable on the spindle, a monitor with a 0-100 health score, no people." caption="IMS Center. Below 50, service. Below 30, the machine was not to be used." credit="Staff" />}}

Mazak’s machines run from the price of a house to the price of a plant. Maintenance is a calendar: the line stops, a checklist walks the spindle, production waits. Predictive maintenance was the bid to call that stop when the signal said so, not when the week did.

**The duties.** Research data-acquisition systems for vibration on a CNC. Integrate a vibration sensor and a current sensor with an acquisition device on an industrial PC. Store the data, network the PC to the machine so a run could be triggered, preprocess and check quality. Extract features, keep the ones that separated healthy from faulty, classify the failure, and emit a health value. Put the output of logistic regression on a web interface as a spindle health score.

**How it was done.** Runs were taken when the machine was new, dry of lubrication, imbalanced, and with a broken spindle. FFT features, principal-component reduction and logistic regression won the classification. Experimental notebooks became production Python and Flask. The research head and a doctoral student sat on the same bench. The appointment ended in December 2018.

A score below 50 meant maintenance. Below 30, the machine was not to be used. Mazak put the monitor into its machines. In September the same year the work stood on a Chicago show floor.

{{< well kind="inline" prompt="Inline, 4:3: a Flask UI with a single health number, industrial PC in the background, documentary." caption="The floor wanted a warning, not a post-mortem." credit="Staff" />}}
