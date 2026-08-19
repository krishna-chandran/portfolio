---
title: "Logs through the ELK stack, so nobody SSHs at two"
date: 2019-06-15
dek: "Filebeat, Metricbeat, grok filters and a Kibana board for people who would rather sleep."
kicker: "IT operations"
dateline: "Farmington Hills"
tags: ['ignio','it-automation','python','powershell','groovy','bash','postgresql','service-now','email','linux', 'cloud-computing','distributed-systems','elasticsearch','logstash','kibana','beats']
categories: ["Information Technology","Data Science"]
---

FARMINGTON HILLS, Mich. — Duplicate tickets and long hunts through logs are a kind of weather in IT operations. The assignment was to thin that weather with an ELK path and a dashboard.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a Kibana dashboard, four panels of logs and metrics, dark theme, no hostnames readable." caption="The board. Filebeat and Metricbeat fed it; grok filters in Logstash decided what counted." src="images/wells/well-kibana.png" />}}

Pipelines took log streams in through Filebeat and Metricbeat. Grok filters in Logstash did the matching. Metrics and analytics landed on a Kibana dashboard. The aim, on the record, was less duplicate work, less troubleshooting by hand, more room for automation.
