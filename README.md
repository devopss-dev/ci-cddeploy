# 🚀 CI/CD Pipeline for Containerized Web Application

## 📌 Project Overview

This project demonstrates the implementation of an **end-to-end CI/CD pipeline** for a containerized web application using DevOps tools. The pipeline automates the process of code integration, quality analysis, containerization, and deployment to a Kubernetes cluster.

This project is designed to simulate a **real-world production deployment workflow**.

---

## 🛠️ Tech Stack

* **Version Control:** Git, GitHub
* **CI/CD Tool:** Jenkins
* **Code Quality:** SonarQube
* **Containerization:** Docker
* **Container Registry:** Docker Hub
* **Orchestration:** Kubernetes
* **Cloud Platform:** AWS EC2 (for hosting tools)

---

## ⚙️ Architecture Flow

1. Developer pushes code to GitHub
2. Jenkins pipeline is triggered automatically
3. Code is analyzed using SonarQube
4. Docker image is built from application code
5. Image is pushed to Docker Hub
6. Kubernetes pulls the latest image
7. Application is deployed using Deployment & Service

---

## 🔄 CI/CD Pipeline Stages

### 1. Code Checkout

* Pulls latest source code from GitHub repository

### 2. Code Quality Analysis

* Runs SonarQube scan to detect bugs and vulnerabilities

### 3. Build Docker Image

* Builds Docker image using Dockerfile

### 4. Push to Docker Hub

* Tags and pushes image to Docker Hub repository

### 5. Deploy to Kubernetes

* Applies Kubernetes manifests (Deployment & Service)
* Updates application with latest image

---

## 📁 Project Structure

```
.
├── Jenkinsfile
├── Dockerfile
├── deployment.yaml
├── service.yaml
├── index.html / app files
└── README.md
```

---

## ▶️ Setup Instructions

### Prerequisites

* Linux server (AWS EC2 recommended)
* Docker installed
* Jenkins installed
* Kubernetes cluster (Minikube / Kubeadm)
* SonarQube server running
* Docker Hub account

---

### Step 1: Clone Repository

```
git clone https://github.com/devopss-dev/ci-cddeploy
cd ci-cddeploy
```

### Step 2: Configure Jenkins

* Install required plugins (Docker, Git, Pipeline)
* Add Docker Hub credentials
* Configure SonarQube in Jenkins

---

### Step 3: Run Pipeline

* Create a Jenkins pipeline job
* Add your `Jenkinsfile`
* Trigger build manually or via GitHub webhook

---

### Step 4: Deploy Application

```
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

---

## 📊 Key Outcomes

* Automated end-to-end deployment process
* Reduced manual intervention in build and deployment
* Improved deployment consistency and reliability
* Enabled scalable application deployment using Kubernetes

---

## 👩‍💻 Author

**Asmiya Amreen Khanam**
DevOps Enthusiast | Aspiring DevOps Engineer.
