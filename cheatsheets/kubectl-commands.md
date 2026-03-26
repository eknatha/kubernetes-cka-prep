# ⚡ Kubectl Commands Cheatsheet

A quick reference guide for commonly used kubectl commands for CKA preparation.

---

## 📌 Cluster Info

```bash
kubectl cluster-info
kubectl get nodes
kubectl get componentstatuses
```

---

## 📌 Get Resources

```bash
kubectl get pods
kubectl get pods -A
kubectl get pods -o wide
kubectl get svc
kubectl get deployments
kubectl get all
```

---

## 📌 Describe & Debug

```bash
kubectl describe pod <pod>
kubectl logs <pod>
kubectl logs -f <pod>
kubectl exec -it <pod> -- /bin/sh
kubectl get events
```

---

## 📌 Create Resources

```bash
kubectl run nginx --image=nginx
kubectl create deployment nginx --image=nginx
kubectl expose deployment nginx --port=80 --type=NodePort
```

---

## 📌 YAML Operations

```bash
kubectl apply -f file.yaml
kubectl create -f file.yaml
kubectl delete -f file.yaml
kubectl run nginx --image=nginx --dry-run=client -o yaml
```

---

## 📌 Scaling & Updates

```bash
kubectl scale deployment nginx --replicas=3
kubectl rollout status deployment nginx
kubectl rollout undo deployment nginx
```

---

## 📌 Namespaces

```bash
kubectl get ns
kubectl create ns dev
kubectl config set-context --current --namespace=dev
```

---

## 📌 ConfigMaps & Secrets

```bash
kubectl create configmap app-config --from-literal=env=prod
kubectl create secret generic db-secret --from-literal=password=1234
```

---

## 📌 Delete Resources

```bash
kubectl delete pod <pod>
kubectl delete deployment <deployment>
kubectl delete svc <service>
```

---

## ⚡ Pro Tips

- Use alias:
  ```bash
  alias k=kubectl
  ```
- Enable autocomplete:
  ```bash
  source <(kubectl completion bash)
  ```

---

## 🎯 Goal

Master these commands to improve speed and accuracy in the CKA exam.
