# 🚀 Kubernetes CKA Prep (21-Day Hands-on Guide)

A structured, hands-on 21-day preparation plan to crack the **Certified Kubernetes Administrator (CKA)** exam with real-world labs, kubectl commands, YAML configurations, and troubleshooting scenarios.

---


![Eknatha](https://img.shields.io/badge/Eknatha-4EAA25?style=flat&logo=gnu-bash&logoColor=white)




## 🎯 Goal
- Master Kubernetes fundamentals and core components
- Build strong hands-on command-line skills
- Practice real exam scenarios
- Crack the CKA exam with confidence

---

## 📚 What You’ll Learn

- Kubernetes Architecture (API Server, Scheduler, etcd)
- Pods, Deployments, ReplicaSets
- Services & Networking
- ConfigMaps & Secrets
- Storage (PV, PVC, StatefulSets)
- Scheduling (Taints, Tolerations, Affinity)
- Troubleshooting (logs, events, debugging)
- Imperative vs Declarative approaches

---

## 🛠️ Prerequisites

- Basic Linux knowledge
- Familiarity with containers (Docker helpful)
- Install:
  - Minikube / Kind
  - kubectl CLI

---

## 📅 21-Day Plan Overview

| Week | Focus Area |
|------|-----------|
| Week 1 | Core Concepts (Pods, YAML, Deployments, Services) |
| Week 2 | Scheduling, Storage, Networking |
| Week 3 | Troubleshooting + Mock Exams |

---

## 📂 Repository Structure

```
kubernetes-cka-prep/
│
├── day01-cluster-setup.md
├── day02-pods.md
├── day03-yaml.md
├── day04-deployments.md
├── day05-services.md
├── ...
│
├── labs/                 # YAML files and hands-on configs
├── troubleshooting/      # Common issues and fixes
├── exam-scenarios/       # Real exam-like scenarios ⭐
├── cheatsheets/          # Quick revision notes ⚡
├── notes/                # Concept explanations 🧠
├── mock-tests/           # Practice exams 🎯
├── scripts/              # Automation scripts 🛠️
├── diagrams/             # Architecture visuals 📊
├── resources/            # Useful links & references 🔗
│
└── README.md
```

---

## 📁 Folder Breakdown

### 🧪 labs/
Contains YAML manifests and practical configurations used during hands-on practice.

### 🐞 troubleshooting/
Real-world Kubernetes issues like:
- CrashLoopBackOff
- ImagePullBackOff
- Debugging pods and services

### 🎯 exam-scenarios/
Practice real CKA-style problems with step-by-step solutions.

### ⚡ cheatsheets/
Quick reference guides for:
- kubectl commands
- YAML templates
- Debugging steps

### 🧠 notes/
Concept-focused notes for revision and interviews.

### 📝 mock-tests/
Time-based practice tests to simulate real exam conditions.

### 🛠️ scripts/
Automation scripts for setup, cleanup, and efficiency.

### 📊 diagrams/
Visual representations of Kubernetes architecture and workflows.

### 🔗 resources/
Curated list of learning materials, tools, and practice platforms.

---

## 🔥 Key Commands You’ll Master

```bash
kubectl get pods
kubectl describe pod <pod>
kubectl logs <pod>
kubectl exec -it <pod> -- /bin/sh
kubectl apply -f file.yaml
kubectl create deployment nginx --image=nginx
kubectl expose deployment nginx --port=80 --type=NodePort
```

---

## ⚡ Exam Tips

- Focus on **hands-on practice (70%)**
- Use **imperative commands** to save time
- Practice YAML editing speed
- Learn to navigate Kubernetes docs quickly
- Troubleshooting skills are critical for passing

---

## 🧪 Practice Strategy

- Repeat labs daily until commands become muscle memory
- Break and fix clusters intentionally
- Simulate exam conditions (time-bound practice)

---

## 📈 Progress Tracking

- ✅ Daily commits
- ✅ Lab completion
- ✅ Notes for each topic
- ✅ Troubleshooting scenarios documented

---

## 🌟 Contribution & Support

If you find this helpful:
- ⭐ Star this repo
- 🍴 Fork and practice
- 📢 Share with others preparing for CKA

---

## 🔗 Connect with Me

- GitHub: https://github.com/eknatha
- LinkedIn: https://linkedin.com/in/eknathareddyp

---

## 🚀 Final Note

This repository is not just about passing the exam — it's about building real-world Kubernetes skills that can be applied in DevOps, SRE, and Platform Engineering roles.

**Consistency + Hands-on Practice = Success 💯**

