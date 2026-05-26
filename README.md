# 🚀 CI/CD DevOps Project

## Project Title
End-to-End CI/CD Pipeline using GitHub, Jenkins, Docker, and Kubernetes

---

## 🎯 Objective
The objective of this project is to automate the complete software delivery process using CI/CD tools. The application is built, containerized, pushed to DockerHub, and deployed on Kubernetes.

---

## 🛠️ Tools & Technologies Used
- GitHub (Source Code Management)
- Jenkins (CI/CD Automation)
- Docker (Containerization)
- DockerHub (Image Registry)
- Kubernetes (Container Orchestration)
- Minikube (Local Kubernetes Cluster)

---

## 🔄 CI/CD Workflow


GitHub → Jenkins → Docker Image → DockerHub → Kubernetes → Browser


---

## ⚙️ Step-by-Step Process

### 1️⃣ Source Code Management
- Code is written using HTML (or application code)
- Uploaded to GitHub repository

---

### 2️⃣ Continuous Integration (Jenkins)
- Jenkins pulls code from GitHub
- Jenkinsfile defines pipeline stages
- Docker image is built automatically

---

### 3️⃣ Docker Image Creation
- Dockerfile is used to build image
- Application is containerized
Command:
docker build -t myapp:latest .

4️⃣ DockerHub Push
Image is tagged and pushed to DockerHub
Commands:
docker tag myapp:latest username/myapp:latest
docker push username/myapp:latest

5️⃣ Kubernetes Deployment
Deployment file is created (deployment.yaml)
Pods are created using Docker image
Command:
kubectl apply -f deployment.yaml

6️⃣ Service Exposure
Kubernetes Service exposes application to browser
Command:
kubectl expose deployment myapp --type=NodePort --port=80

🌐 Final Output
Hello DevOps  
My First CI/CD Pipeline Project
