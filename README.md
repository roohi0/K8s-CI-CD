 🚀 End-to-End CI/CD Pipeline for Nginx Application using Jenkins & Kubernetes

📌 Project Overview

This project demonstrates an end-to-end CI/CD pipeline for deploying a containerized Nginx web application on a Kubernetes cluster using Jenkins.

The pipeline automates the deployment of Kubernetes manifests including Deployment, Service, and Horizontal Pod Autoscaler (HPA).


🛠️ Technologies Used

- Docker
- Nginx
- Kubernetes
- Jenkins
- Git & GitHub
- Linux (Ubuntu)

 📁 Project Structure
 
 nginx-k8s-ci-cd-project/
│
├── Dockerfile
├── Jenkinsfile
├── index.html
│
└── k8s/
├── nginxdep.yaml
├── hpatask.yaml
└── svc.yaml


🐳 Docker

- Created a custom Docker image using Nginx
- Hosted a simple static web page
- Image pushed to Docker Hub


☸️ Kubernetes Configuration

  1️⃣ Deployment
    - 2 replicas
    - CPU resource limits defined
    - Container port: 80

  2️⃣ Horizontal Pod Autoscaler (HPA)
    - Min replicas: 2
    - Max replicas: 5
    - CPU utilization based scaling

  3️⃣ Service
    - Type: NodePort
    - Exposes application externally

🔄 Jenkins Pipeline

The Jenkins pipeline:

- Connects to Kubernetes cluster using KUBECONFIG
- Deploys Kubernetes manifests automatically

🎯 Key Features

✔ Containerized Application  
✔ Automated Deployment using Jenkins  
✔ Kubernetes Deployment & Service  
✔ Horizontal Pod Autoscaling  
✔ Infrastructure as Code  
✔ Version Controlled via Git  

📌 How to Run the Project

1. Clone repository
2. Build & push Docker image
3. Configure KUBECONFIG in Jenkins
4. Run Jenkins pipeline
5. Access application using NodePort


👩‍💻 Author

Roohi  
DevOps Enthusiast 🚀
