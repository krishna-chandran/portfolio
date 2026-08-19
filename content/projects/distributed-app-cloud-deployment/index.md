---
title: "Twelve VMs, one playbook, ignio in high availability"
date: 2020-01-10
dek: "Ansible from capacity checks through Hadoop, Neo4j and ELK, then Enigma to say it was true."
kicker: "IT operations"
dateline: "Farmington Hills"
tags: ['linux','aws','azure','ansible','ignio','high-availability','ssl','pgpool','hadoop','haproxy','it-automation','bash','postgresql','rabbitmq','kafka','vmware','cloud-computing','distributed-systems','eureka','neo4j','hdfs','yarn','zookeeper','elasticsearch','logstash','kibana','beats']
categories: ["Information Technology"]
---

FARMINGTON HILLS, Mich. — The assignment was to land ignio in high availability across a distributed cloud: twelve Linux VMs, a playbook for each layer, and a check at the end that did not trust a hopeful engineer.
<!--more-->

{{< well kind="lead" prompt="Wide, 16:9: a rack row and a laptop with an Ansible run scrolling, no cloud-console screenshots with account IDs." caption="Twelve machines. Java, Postgres, Hadoop, Neo4j, then the application itself." credit="Staff" />}}

Ansible scripts validated VM capacity and prerequisites, provisioned Linux in the cloud, then handled IAM, LDAP, security roles, filesystems and patching. The same tool installed Java JRE, PostgreSQL, Hadoop pieces and Neo4j on all twelve boxes, then the Java application, services, configuration, and Elasticsearch, Logstash and Kibana. Enigma, an Ansible-powered checker, ran the deployment validation.
