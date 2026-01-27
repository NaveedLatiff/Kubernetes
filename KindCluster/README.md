# My Kubernetes Learning – Kind Cluster

Hi! This folder contains my hands-on experiments with **Kind**, which is Kubernetes running locally in Docker.  
I’m using this setup to learn how clusters work, understand master & worker nodes, and practice deploying applications.


## What I Learned
 Kind lets me create **multi-node Kubernetes clusters** locally.
 I can simulate **1 control-plane node (master) + 3 worker nodes** using Docker containers.
 I practiced **kubectl commands, deployments, services, and port-forwarding** without using any cloud resources.



## Commands I Used to Create Cluster

# Check Kind version
kind --version

# Create cluster from YAML
kind create cluster --name kind_cluster --config kind-cluster.yaml

# See the nodes
kubectl get nodes

# Delete cluster when done
kind delete cluster --name kind_cluster

# Kubectl Commands I Practiced

# List all nodes
kubectl get nodes


