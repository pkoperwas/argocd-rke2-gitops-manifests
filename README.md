# 🚀 argocd-rke2-gitops-manifests

![GitOps](https://img.shields.io/badge/GitOps-ArgoCD-blue)
![Kubernetes](https://img.shields.io/badge/K8s-RKE2-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

This repository contains **GitOps manifests for RKE2 Kubernetes clusters** using **ArgoCD**.  
It provides a structured way to manage applications and ArgoCD configuration declaratively.

---

## 📂 Repository Structure

### 🗂 argocd-applicationset
- Contains **ArgoCD ApplicationSet definitions**  
- Configures ArgoCD to automatically deploy applications based on Git repository content  
- Enables automated sync and requeue for cluster applications

### 🗂 apps
- Contains **application manifests** (deployments, services, ingresses, PVCs, etc.)  
- Each application is managed independently  
- Keeps the GitOps workflow modular and maintainable

---

## ⚡ Purpose
- Centralized **configuration for ArgoCD** on RKE2 clusters  
- Automates application deployment using GitOps principles  
- Simplifies management of multiple applications across clusters  
- Ensures **declarative and reproducible infrastructure**

---

## 🔧 How to Use
1. Clone the repository to your GitOps control cluster.  
2. ArgoCD watches `argocd-applicationset` and `apps` directories.  
3. Changes pushed to Git are automatically applied to the cluster via ArgoCD.

---

## 💡 Highlights
- 🟢 Fully GitOps-driven workflow  
- 🟢 Supports multiple clusters and applications  
- 🟢 Modular structure for easy scaling  
- 🟢 Declarative infrastructure for reproducibility

---

## 📚 References
- [ArgoCD Documentation](https://argo-cd.readthedocs.io/)  
- [RKE2 Kubernetes](https://docs.rke2.io/)  
- GitOps principles: declarative, version-controlled, automated
