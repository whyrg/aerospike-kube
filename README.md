# aerospike-kube

This repo is no longer maintained and serves as a learning/experiemental repo. The officially supported repo is over at:
https://github.com/aerospike/aerospike-kubernetes.

This project contains the init container used in Kubernetes (k8s) and the aerospike petset definition

## Usage:

Configure `image/aerospike.conf` for your aerospike cluster.

Build and push the aerospike-install container to the Docker registry of your choice (See image/README.md)

Use the aerospike-install image as the init-container for the PetSet

Deploy the petset: `kubectl create -f aerospike-petset.yaml`

## Requirements

* Kubernetes 1.3+ with alpha features (PetSet, init containers)
* Kubernetes DNS add-in

