# 🚀 DevOps Project: ZOMATO Clone App Deployment

This project demonstrates a complete **End-to-End DevOps CI/CD pipeline** for deploying a Zomato Clone application using modern DevOps tools and practices.

---

## 🛠️ Tools & Technologies Used

- **Git & GitHub** – Source Code Management  
- **Jenkins** – CI/CD Pipeline Automation  
- **Docker** – Containerization  
- **Docker Hub** – Image Repository  
- **Kubernetes** – Container Orchestration  
- **ArgoCD** – GitOps Continuous Deployment  
- **Trivy** – Security Scanning  
- **OWASP Dependency Check** – Vulnerability Analysis  
- **Prometheus & Grafana** – Monitoring & Visualization  

---

## 📌 Project Workflow

### 🔹 Stage 1: CI Pipeline
- Code pushed to GitHub
- Jenkins pipeline triggered automatically
- Build and test application
- Docker image created

### 🔹 Stage 2: Dockerization
- Application containerized using Docker
- Image pushed to Docker Hub

### 🔹 Stage 3: Kubernetes Deployment
- Application deployed on Kubernetes cluster
- Services exposed using NodePort

### 🔹 Stage 4: GitOps with ArgoCD
- Automated deployment from GitHub repository
- Continuous synchronization with Kubernetes cluster

### 🔹 Stage 5: Monitoring & Security
- Application monitored using Prometheus & Grafana
- Security scanning using Trivy & OWASP

---

## 📂 Repository Structure
