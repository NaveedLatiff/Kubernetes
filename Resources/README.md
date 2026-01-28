# Kubernetes Resources Lab

This folder contains all the YAML files and commands I practiced today to learn Kubernetes objects.  
I focused on creating **Namespaces, Pods, Deployments, ReplicaSets, and DaemonSets** and using **kubectl commands** to manage them.

---

## Commands Practiced Today

### Namespace
```bash
kubectl apply -f namespace.yaml
kubectl get ns
kubectl delete ns nginx
kubectl apply -f pod.yaml
kubectl get pods -n nginx
kubectl exec -it nginx-pod -n nginx -- bash
kubectl delete pod nginx-pod -n nginx
kubectl apply -f deployment.yaml -n nginx
kubectl get deployments -n nginx
kubectl scale deployment/nginxdeployment -n nginx --replicas=5
kubectl set image deployment/nginxdeployment nginx=nginx:1.21.0 -n nginx
kubectl rollout status deployment/nginxdeployment -n nginx
kubectl rollout undo deployment/nginxdeployment -n nginx
kubectl delete deployment nginxdeployment -n nginx
kubectl get pods -n nginx -o wide
