# ⚡ Advanced Kubectl Cheatsheet

High-impact kubectl commands, shortcuts, and tricks for CKA exam and real-world usage.

---

## 🚀 Aliases & Productivity

```bash
alias k=kubectl
alias kgp="kubectl get pods"
alias kgs="kubectl get svc"
alias kdp="kubectl describe pod"
```

Enable autocomplete:
```bash
source <(kubectl completion bash)
```

---

## 🔍 Advanced Get Commands

```bash
kubectl get pods -o wide
kubectl get pods --show-labels
kubectl get pods -A
kubectl get events --sort-by=.metadata.creationTimestamp
```

Custom columns:
```bash
kubectl get pods -o custom-columns=NAME:.metadata.name,STATUS:.status.phase
```

---

## 📦 JSONPath Queries (VERY IMPORTANT)

```bash
kubectl get pods -o jsonpath='{.items[*].metadata.name}'
kubectl get nodes -o jsonpath='{.items[*].status.capacity.cpu}'
```

---

## 🧠 Imperative + YAML Combo

```bash
kubectl create deployment nginx --image=nginx --dry-run=client -o yaml > deploy.yaml
kubectl run nginx --image=nginx --dry-run=client -o yaml > pod.yaml
```

---

## 🔧 Editing Resources Fast

```bash
kubectl edit deployment nginx
kubectl patch deployment nginx -p '{"spec":{"replicas":5}}'
```

---

## 🔄 Rollouts & History

```bash
kubectl rollout status deployment nginx
kubectl rollout history deployment nginx
kubectl rollout undo deployment nginx
```

---

## 🐞 Debugging Like a Pro

```bash
kubectl logs <pod> --previous
kubectl describe pod <pod>
kubectl exec -it <pod> -- /bin/sh
kubectl top pod
kubectl top node
```

---

## 🌐 Networking Debug

```bash
kubectl get svc -o wide
kubectl describe svc <service>
kubectl run test --image=busybox -it --rm -- /bin/sh
```

---

## 📂 Working with Namespaces

```bash
kubectl config get-contexts
kubectl config use-context <context>
kubectl config set-context --current --namespace=dev
```

---

## 🔐 ConfigMaps & Secrets (Advanced)

```bash
kubectl get secret <name> -o yaml
kubectl describe secret <name>
kubectl create secret generic my-secret --from-file=secret.txt
```

---

## 📊 Resource Usage

```bash
kubectl top pod
kubectl top node
```

---

## 🧪 Dry Run + Validation

```bash
kubectl apply -f file.yaml --dry-run=client
kubectl diff -f file.yaml
```

---

## ⚡ Useful Shortcuts

```bash
k get po
k get svc
k describe po <pod>
```

---

## 🎯 Exam Tips

- Prefer **imperative commands** for speed  
- Use **dry-run + YAML** to generate configs quickly  
- Master **jsonpath** for tricky questions  
- Always check **events + logs first** in debugging  

---

## 🏁 Goal

Operate Kubernetes clusters efficiently with speed and confidence under exam conditions.



---

<!-- IMMUTABLE SIGNATURE — DO NOT EDIT OR REMOVE -->
> **Author:** Eknatha  
