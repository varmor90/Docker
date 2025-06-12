# ☁️ Laravel Docker Deployment – AWS Cloud

This directory contains the **cloud deployment layer** for my Laravel Docker project.

I deployed a multi-container Laravel application to **AWS** using a mix of **manual and managed services** (EC2, ECS, ALB, ECR, MongoDB Atlas). This was part of a deeper learning process aimed at understanding how local Docker development can transition into a real-world cloud deployment setup.

---

## 🔧 What This Includes

✅ **Building and pushing Docker images to Amazon ECR**  
✅ **Manual EC2 deployment** with Docker installed  
✅ Deployment using **AWS ECS Fargate** for container orchestration  
✅ Integration with **Application Load Balancer (ALB)**  
✅ Switching from MySQL to **MongoDB Atlas** in production  
✅ Use of **EFS volumes** for shared, persistent storage  
✅ Implementing **multi-stage builds** for leaner production images  
✅ Managing `dev` vs `prod` environment differences  
✅ Handling secrets and environment variables

---

## 🚀 Deployment Steps Covered

1. ✅ Install Docker on EC2
2. ✅ Push image from local to Amazon ECR
3. ✅ Run container manually (initial test)
4. ✅ Define and launch ECS Task Definitions & Services
5. ✅ Configure ALB for public access
6. ✅ Set up persistent data (EFS / MongoDB Atlas)
7. ✅ Use environment variables for production settings
8. ✅ Deploy multi-container setup with ECS + ALB
9. ✅ Update and manage deployments using versioned images

---

## 🛠️ Tools & Services Used

- **Docker** (build, tag, push, run)
- **AWS EC2** (manual deployment base)
- **AWS ECS (Fargate)** for container orchestration
- **AWS ECR** (container registry)
- **Application Load Balancer**
- **MongoDB Atlas** (managed database)
- **Amazon EFS** (persistent volume for containers)

---

## 🧠 Lessons Learned

- How to go from `docker-compose` to production-ready Docker images
- How to decouple database setup by moving to managed DB services
- Challenges of managing secrets, volumes, and networking in cloud
- Importance of multi-stage builds and image size optimization
- Real-world differences between development and production Docker setups

---

## 📁 Folder Contents

