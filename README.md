# 🧪 Laravel Docker Lab – Dev & Deployment

This repository documents my **DevOps learning lab**, where I containerized a Laravel application, ran it locally with Docker Compose, and then deployed it to the **AWS Cloud** using ECS, ECR, ALB, and other services.

---

## 📁 Project Structure

├── docker-project/ ← Local development setup using Docker Compose
└── docker-deployment/ ← Cloud deployment setup using AWS (ECS, ECR, ALB, MongoDB Atlas)


---

## 📦 What's inside

### `docker-project/`
A fully Dockerized Laravel 12 application using:
- Nginx + PHP-FPM + MySQL
- Utility containers: Composer, Artisan, NPM
- Clean architecture with working volume management and permission handling

### `docker-deployment/`
Production deployment resources covering:
- Docker image build & push to Amazon ECR
- Manual deployment on EC2
- Managed deployment on AWS ECS Fargate
- Application Load Balancer integration
- Use of MongoDB Atlas and EFS volumes
- Multi-stage Docker builds and dev/prod config handling

---

## 🎯 Goal

To understand how to:
- Move from local Docker-based development to cloud deployment
- Solve real-world DevOps problems (timing, environment configs, volumes, secrets)
- Learn the cloud-native way of deploying PHP/Laravel apps using AWS services

This lab lays the groundwork for future expansion into **Kubernetes**

---

