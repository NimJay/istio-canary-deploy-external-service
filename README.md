# Istio Canary Deployment of External Service

This repository contains YAML samples for the following scenario:
* You have a version 1 of a "Hello, world!" app running inside your Kubernetes cluster.
* You have a version 2 of the same app running outside your Kubernetes cluster, at a public (accessible through the Internet) IP address.
* You want to perform a canary deployment of version 2, so you split 75% of the traffic to version 1 and 25% of the traffic to version 2.
* Internet users come to your "Hello, world!" app through http://example.com:80.

![Diagram of a Kubernetes cluster containing running two Pods — a "Hello, world!" Pod and the Istio ingress gateway Pod.](https://github.com/NimJay/istio-canary-deploy-external-service/raw/main/diagram.png)
