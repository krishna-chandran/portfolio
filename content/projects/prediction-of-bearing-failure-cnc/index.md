---
title: "A Mazak spindle, scored from 0 to 100"
date: 2018-12-15
dek: "FFT, PCA, logistic regression, and a Flask app — funded by Mazak, shown at IMTS Chicago."
kicker: "Industrial AI"
dateline: "Cincinnati"
tags: ['python','matlab','flask','machine-learning']
categories: ["Data Science"]
---

CINCINNATI — Mazak’s machines cost what a shop cannot casually idle. Weekly and monthly checklists stop the spindle on a calendar. The 2018 project, funded by Mazak, asked whether vibration and current could call maintenance before the calendar did.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a bearing, a vibration cable, and a 0-100 health plot, lab bench, no vendor marks." caption="Below 50, service. Below 30, stop. The floor wanted a number, not a paper." src="images/wells/well-bearing.png" />}}

Sensors went on a Mazak CNC through Advantech acquisition. Runs were taken healthy, dry, imbalanced and broken. Features were pulled from the time series; FFT, principal components and logistic regression classified health from fault.

A web application showed the score live. Mazak put the monitor on machines. IMTS Chicago, 2018, carried the banner for Mazak and the IMS lab. [The university’s note](https://www.uc.edu/news/articles/2019/01/n2063491.html) followed in January 2019.
