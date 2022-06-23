---
title: Cloud Native Storage
status: Completed
category: concept
---

## What it is

The **general definition** of cloud-native storage refers to storage systems that

1. Deploy on Kubernetes
1. Serve application POD on Kubernetes

which includes all the key/value stores, object stores, databases and block/file storages that are containerized and running on Kubernetes.

The **strict definition** of cloud-native storage further requires storage systems:

3. Employ Kubernetes CSI (Container Storage Interface)
4. Store internal key/value in Kubernetes CRD

which only includes the storages that are deeply integrated to Kubenretes and directly provide backends to Kubernetes persistent volume objects.

Details about cloud-native storage landscapes are documented in CNCF Storage Whitepaper: [ https://bit.ly/cncf-storage-whitepaperV2 ]( https://bit.ly/cncf-storage-whitepaperV2)

## Problem it addresses

Cloud native architecture requires storage services to automate according to container scheduling and application needs.

Traditional storages operates in their own hardware environments which are isolated from Kubernetes, therefore cannot respond to cloud-native operations effectively.

## How it helps

Cloud-native storages live on Kubernetes and use hardware in the Kubernetes nodes. This natural hyper-convergence enables data affinity, which places data close to the applications for faster access.

Cloud-native storages scale with Kubernetes clusters, which eliminates structural bottlenecks.

Cloud-native applications may directly coordinate with cloud-native storages to automate operations such as snapshot, backup&restore.
