---
kind: work
title: "Krishna joins the IMS lab to ask a Mazak spindle to confess early"
date: 2018-07-22
dek: "Full-stack engineer: pick the acquisition hardware, classify the fault, show logistic regression as a 0–100 score."
kicker: "Work"
dateline: "Cincinnati"
skills: ["python","flask","matlab","scikit-learn"]
fields: ["Machine Learning","Physical AI"]
---

CINCINNATI — On 22 July 2018 Krishnakumar Chandran joined the Intelligent Maintenance Systems laboratory as a full-stack engineer. Mazak funded the project. The appointment ended on 15 December 2018. The objective was to predict CNC spindle failure before the floor hears it.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a Mazak CNC in a university lab, vibration cable on the spindle, a monitor with a 0-100 health score, no people." caption="Below 50, service. Below 30, stop." src="images/wells/well-cnc-lab.png" />}}

Mazak’s machines run from about a hundred thousand dollars to about ten million. Maintenance is a calendar. A vibration sensor and a current sensor went onto the machine and into Advantech acquisition on an industrial PC. Data was taken when the machine was new, dry of lubrication, imbalanced, and with a broken spindle. FFT features, principal-component reduction and logistic regression won the classification. Experimental notebooks became production Python and Flask. A web score from 0 to 100: below 50, service; below 30, the machine was not to be used.

Mazak put the monitor into its machines. IMTS Chicago, September 2018. The university [wrote it up](https://www.uc.edu/news/articles/2019/01/n2063491.html) the following January.
