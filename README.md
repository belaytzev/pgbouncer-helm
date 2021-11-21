# Helm Chart for PgBouncer

## Introduction

 - This [Helm](https://helm.sh/) chart installs [pgbouncer](http://www.pgbouncer.org) in a Kubernetes cluster.
 - Inspired by [cradlepoint](https://github.com/cradlepoint/kubernetes-helm-chart-pgbouncer) based on image [pgbouncer/pgbouncer](https://hub.docker.com/r/pgbouncer/pgbouncer)
## Prerequisites

- Kubernetes cluster 1.14.10+
- Helm 2.8.0+

## Installation

### Add Helm repository

```bash
helm repo add belaytzev-pgbouncer https://belaytzev.github.io/pgbouncer-helm
helm repo update
```

### Install the chart

Install the pgbouncer helm chart with a release name `my-release`:

```bash
helm install --name my-release belaytzev-pgbouncer/pgbouncer
```

## Uninstallation

To uninstall/delete the `my-release` deployment:

```bash
helm delete --purge my-release
```
