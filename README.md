# 🚀 Blue-Green Deployment on AWS with CI/CD

## 📌 Project Overview

This project demonstrates a **Blue-Green Deployment strategy** using AWS to achieve **zero downtime deployments**. It integrates CI/CD pipelines, containerization, and load balancing to simulate a real-world production environment.

---

## 🏗️ Architecture

* **EC2 Instances**: Blue (current) & Green (new version)
* **Application Load Balancer (ALB)**: Routes traffic between environments
* **Docker**: Containerized application
* **GitHub Actions**: CI/CD automation
* **Docker Hub**: Image registry

---

## ⚙️ Workflow

1. Developer pushes code to GitHub
2. GitHub Actions pipeline triggers
3. Docker image is built and pushed to Docker Hub
4. Application is deployed to the **Green environment**
5. Green environment is validated manually
6. Traffic is switched from Blue → Green via ALB
7. Rollback possible by switching back to Blue

---

## 🔄 Deployment Flow

```
User → ALB → Blue (Live)
              Green (New Version)

CI/CD → Deploy to Green → Verify → Switch Traffic
```

---

## 🛠️ Tech Stack

* AWS EC2, ALB
* Docker
* GitHub Actions
* Docker Hub

---

## 🔐 Key Features

* Zero downtime deployment
* Manual traffic switching for safe releases
* Instant rollback capability
* CI/CD automated deployment to Green

---

## 🚀 Future Improvements

* Automate ALB traffic switching
* Add CloudWatch monitoring
* Infrastructure provisioning using Terraform
* Upgrade to Kubernetes (EKS)

---

## 💡 Learnings

* Understanding Blue-Green deployment architecture
* CI/CD pipeline design and execution
* Load balancing and traffic routing
* Safe deployment and rollback strategies

---

## 📬 Connect With Me

Feel free to connect on LinkedIn for discussions on DevOps and Cloud 🚀
