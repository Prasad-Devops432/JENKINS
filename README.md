# 🚀 Jenkins CI/CD Projects – End‑to‑End DevOps Pipelines

This repository contains multiple **Jenkins CI/CD pipeline projects** demonstrating real‑world DevOps workflows including **Maven builds, Docker pipelines, SonarQube scanning, Kubernetes deployments, ArgoCD GitOps, multi‑agent pipelines, shared libraries**, and more.

Each folder represents a hands‑on Jenkins automation scenario designed to help you master CI/CD from beginner to advanced level.

---

## 📁 Repository Structure

### **1. my-first-pipeline/**
A simple beginner‑friendly Jenkins pipeline demonstrating:
- Basic pipeline syntax  
- Stages (Build → Test → Deploy)  
- Console output  
- Understanding Jenkinsfile structure  

**Skills:** Declarative Pipeline, Jenkins basics

---

### **2. java-maven-sonar-argocd-helm-k8s/**
A complete enterprise‑style CI/CD pipeline:
- Build Java app using **Maven**
- Run **unit tests**
- Perform **SonarQube code quality scan**
- Build & push **Docker image**
- Deploy to Kubernetes using:
  - **Helm charts**
  - **ArgoCD GitOps automation**

**Skills:** Maven, SonarQube, Docker, Helm, Kubernetes, ArgoCD, GitOps

---

### **3. python-jenkins-argocd-k8s/**
A Python application pipeline including:
- Python dependency installation  
- Unit testing  
- Docker image build  
- Push to registry  
- ArgoCD auto‑sync deployment  

**Skills:** Python, Docker, Kubernetes, ArgoCD

---

### **4. multi-stage-multi-agent/**
A Jenkins pipeline using **multiple agents**:
- Build on one agent  
- Test on another  
- Deploy from a dedicated deploy agent  
- Demonstrates distributed CI/CD architecture  

**Skills:** Jenkins agents, Node labels, Multi‑stage pipelines

---

### **5. shared-libraries/**  
Reusable Jenkins Shared Library:
- Custom global functions  
- Reusable pipeline steps  
- `vars/` folder with Groovy scripts  
- Helps avoid duplicate code across pipelines  

**Skills:** Groovy, Jenkins Shared Libraries, DRY pipelines

---

### **6. vars/**  
Contains Groovy functions used by the shared library:
- Logging functions  
- Build helpers  
- Deployment helpers  

**Skills:** Groovy scripting, Jenkins automation

---

## 🧰 Tools & Technologies

| Category | Tools |
|---------|-------|
| **CI/CD** | Jenkins, Shared Libraries, Multi‑Agent Pipelines |
| **Build Tools** | Maven, Python, npm |
| **Containers** | Docker, Docker Hub |
| **Quality** | SonarQube |
| **Kubernetes** | Helm, ArgoCD, GitOps |
| **Cloud** | AWS EC2 (Jenkins Master & Agents) |

---

## 🏗️ Example Jenkinsfile (General Structure)

```groovy
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Docker Build & Push') {
            steps {
                echo "Building Docker image..."
            }
        }

        stage('Deploy to Kubernetes') {
            steps {
                echo "Deploying using Helm/ArgoCD..."
            }
        }
    }
}
```

---

## 🚀 How to Use This Repository

### **Clone the repo**
```bash
git clone https://github.com/Prasad-Devops432/JENKINS.git
cd JENKINS
```

### **Choose a project folder**
Example:
```bash
cd java-maven-sonar-argocd-helm-k8s
```

### **Create a Jenkins Pipeline**
1. Open Jenkins → New Item  
2. Select **Pipeline**  
3. Choose **Pipeline from SCM**  
4. Paste your repo URL  
5. Select the folder containing the Jenkinsfile  

---

## 🎯 Purpose of This Repository

This repo is designed to:
- Demonstrate **real DevOps CI/CD pipelines**
- Showcase your **hands‑on Jenkins experience**
- Provide recruiters with **clear project examples**
- Help you practice **enterprise‑level automation**

---
