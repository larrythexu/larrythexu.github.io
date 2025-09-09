---
title: "Reliable Web Service Demo :microscope:"
layout: post
date: 2025-09-08
headerImage: false
projects: true
hidden: false
description: "Creating a Flask Live WebApp with Kubernetes and Docker"
category: project
author: Lawrence Xu
externalLink: false
---

Tools and Skills:
 - Kubernetes
 - Docker
 - Github Actions
 - Prometheus
 - Grafana
 - PostgreSQL

 [Github Link](https://github.com/larrythexu/ReliableWebDemo)

---

This project was to dial up my knowledge in Kubernets and Docker. This was to learn how to set something up in my own cluster, manage the deployments, and adding Services/Ingress/Monitor objects. At work, I interacted with K8s but I never fully controlled everything. Doing this to **really** grasp it.

Also explored Prometheus and Grafana integration to help with live monitoring. It's still in the works, I'm currently learning more about configuring a Postgres DB with it and volume mounts.

![K8s Pod Logs](https://raw.githubusercontent.com/larrythexu/ReliableWebDemo/refs/heads/main/imgs/day2-liveness.png)

![Grafana Logs](https://raw.githubusercontent.com/larrythexu/ReliableWebDemo/refs/heads/main/imgs/day3%20-%20grafana%20metrics.png)
