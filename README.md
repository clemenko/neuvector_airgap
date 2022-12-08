---
title: Air Gapping Neuvector for Fun
author: Andy Clemenko, @clemenko, andy.clemenko@rancherfederal.com
---

# Air Gapping Neuvector for Fun

![logp](img/rancher-neuvector.png)

This guide is very similar to [Simple RKE2, Neuvector, Longhorn, and Rancher Install ](https://github.com/clemenko/rke_install_blog), except in one major way. This guide will provide a strategy for air gapping all the bits needed for RKE2, Longhorn and Rancher. This is just one opinion. We are starting from the idea that there is no container infrastructure available.

Throughout my career there has always been a disconnect between the documentation and the practical implementation. The Kubernetes (k8s) ecosystem is no stranger to this problem. This guide is a simple approach to installing Kubernetes and some REALLY useful tools. We will walk through installing all the following.

- [RKE2](https://docs.rke2.io) - Security focused Kubernetes
- [Rancher](https://www.suse.com/products/suse-rancher/) - Multi-Cluster Kubernetes Management
- [Longhorn](https://longhorn.io) - Unified storage layer
- [Neuvector](https://neuvector.com/) - Kubernetes Security Platform

We will need a few tools for this guide. Hopefully everything at handled by my [air_gap_all_the_things.sh](https://github.com/clemenko/rke_airgap_install/blob/main/air_gap_all_the_things.sh) script. For this guide all the commands will be in the script.

---

> **Table of Contents**:
>
> * [Whoami](#whoami)
> * [Prerequisites](#prerequisites)