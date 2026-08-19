---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
dek: ""
kicker: "Dispatch"
dateline: "Cincinnati"
draft: true
categories: ["Dispatch"]
---

Lead graf.
<!--more-->

{{ "{{< well kind=\"lead\" prompt=\"Describe the picture to shoot or generate.\" caption=\"Cutline.\" />}}" | safeHTML }}

Body graf.
