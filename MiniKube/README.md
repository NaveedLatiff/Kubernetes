# Kubernetes Learning – Minikube Cluster

Hi! This folder contains my experiments with **Minikube**, which lets me run a Kubernetes cluster locally on my machine.  
I’m using this to practice deployments, services, and kubectl commands without spending money on cloud resources.



## What I Learned
- Minikube creates a **single-node or simulated multi-node cluster** locally.  
- I can deploy applications, expose services, and test networking.  
- It’s perfect for practicing Kubernetes concepts before moving to real clusters.



# Start a single-node cluster
minikube start

# Start a multi-node cluster (simulation)
minikube start --nodes=3 -p myminikube

# Check cluster status
minikube status
