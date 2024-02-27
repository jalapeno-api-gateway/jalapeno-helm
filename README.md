<h1 align="center">Jalapeno Helm Chart</h1>
<p align="center">
	<img src="https://github.com/cisco-open/jalapeno/blob/main/docs/img/jalapeno_architecture.png">
</p>

<p align="center">
This repository contains the helm chart to deploy Jalapeno on a Kubernetes cluster.
The official repository for Jalapeno can be found <a href="https://github.com/cisco-open/jalapeno">here</a>.
</p>

---

## Requirements
In order to use the Helm chart as is, a Kubernetes load balancer is needed.

## Installation
1. Create namespace "jalapeno" on cluster
2. Install using files locally ``helm install jalapeno ./jalapeno-helm -n jalapeno``

## Changes to ArangoDB
If the arangoDB gets changed the ArangoDB Chart has to be rebuild and copied into the charts folder of the Jalapeno Chart.

- build ArangoDB Chart: ``helm package .``
