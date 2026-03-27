# Deployment Template

Basic Kubernetes Deployment YAML template for managing application replicas.

## Usage

- Create and manage multiple pod replicas  
- Perform rolling updates and rollbacks  
- Modify image, replicas, and labels as needed  

## Apply

```bash
kubectl apply -f deployment.yaml
kubectl get deployments
kubectl get pods
