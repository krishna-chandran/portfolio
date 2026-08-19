---
kind: work
title: "Krishna joins the IMS lab to ask a Mazak spindle to confess early"
date: 2018-07-22
dek: "A full-stack engineer on a Mazak-funded project: vibration, current, a classifier, and a health score from 0 to 100."
kicker: "Work"
dateline: "Cincinnati"
event: true
categories: ["Industrial AI"]
---

CINCINNATI — On 22 July 2018 Krishnakumar Chandran joined the Intelligent Maintenance Systems laboratory at the University of Cincinnati as a full-stack engineer. The project was funded by Mazak Corporation. The objective was to predict CNC spindle failure before the floor hears it. The appointment ran through 15 December 2018, inside the master’s year.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a Mazak CNC in a university lab, vibration cable on the spindle, a monitor with a 0-100 health score, no people." caption="IMS Center. Below 50, service. Below 30, the machine was not to be used." credit="Staff" />}}

Mazak’s machines run from about a hundred thousand dollars to about ten million. Maintenance is a calendar: the line stops, a checklist walks the spindle, production waits — weekly, monthly, yearly. Predictive maintenance was the bid to call that stop when the signal said so, not when the week did, and to keep a machine alive longer than a checklist would.

He sat the job end to end, as a full-stack engineer translating research-grade models into something a factory could run. First he researched data-acquisition systems for vibration on a CNC, then chose sensors that would give a clean enough signal. A vibration sensor and a current sensor went onto the machine and into Advantech acquisition hardware on an industrial PC. The PC was networked to the CNC so a run could be triggered. Data was stored, preprocessed and checked for quality before anyone trusted a feature.

Runs were taken when the machine was new, dry of lubrication, with tool imbalance, and with a broken spindle. Statistical features were pulled from the time series at several sampling frequencies. Papers in the field supplied the feature list; he kept the ones that actually separated healthy from faulty. The problem was framed as classification: what kind of failure, and what health value.

Data augmentation and transforms sat in the middle of that work. FFT features, principal-component reduction and logistic regression won the bake-off. Experimental notebooks became production Python and Flask. A web interface showed the health score from 0 to 100. Below 50 meant maintenance. Below 30, the machine was not to be used. The research head and a doctoral student sat on the same bench.

Mazak put the monitor into its machines. In September the same year the work stood on the IMTS floor in Chicago, with Mazak and the IMS lab on the banner. The university [wrote it up the following January](https://www.uc.edu/news/articles/2019/01/n2063491.html). The contribution on the file is not a new theorem. It is a research model that left the lab and ran in a shop.

{{< well kind="inline" prompt="Inline, 4:3: a Flask UI with a single health number, industrial PC in the background, documentary." caption="The floor wanted a warning, not a post-mortem." credit="Staff" />}}
