# 🚀 Laravel Dockerized Stack - Learning Project

This repository contains my **hands-on learning project**, where I built a full **Laravel application stack using Docker Compose**.

The goal was not just to "follow the steps", but to really understand:
- how to structure a multi-container Docker setup
- how to containerize PHP applications
- how to manage common real-world challenges (permissions, timing, session handling)
- and how to prepare a project that could be extended towards production deployment.

---

## ⚙️ Stack Overview

- **Laravel** 12 (latest at time of writing)
- **PHP** 8.2-fpm-alpine
- **MySQL** 5.7
- **Nginx** stable-alpine
- **Composer** utility container
- **Artisan** utility container
- **NPM** utility container

---

## 🔍 What I Focused On

✅ Designing a **clean Docker Compose architecture**  
✅ Making sure each component has its own container:
- nginx as web server
- php-fpm for Laravel
- mysql as database
- composer, artisan, npm as utility containers

✅ Solving typical issues:
- Permissions (Laravel storage/cache)
- MySQL startup timing
- SESSION_DRIVER configuration
- How and when to use utility containers

✅ Testing and verifying full Laravel stack under:
- WSL2 (Ubuntu)
- Docker Desktop
- Docker Compose v2

---

## 📚 What was built

Over the course of this project, I gradually implemented:

✅ Nginx container serving Laravel (via `/public`)  
✅ PHP-FPM container with optimized build  
✅ MySQL container with environment-driven config  
✅ Composer container to install Laravel and manage dependencies  
✅ Artisan container for Laravel CLI (migrate, seed, etc.)  
✅ NPM container for building frontend assets

---

## 🏗️ Project Structure

docker-project/
├── docker-compose.yaml
├── dockerfiles/
│ ├── php.dockerfile
│ └── composer.dockerfile
├── nginx/
│ └── nginx.conf
└── src/ ← Laravel 12 application

📓 Notes
✅ For development, SESSION_DRIVER is set to file to simplify local startup.
✅ MySQL migrations completed successfully.
✅ Laravel welcome page loads correctly.
✅ Stack tested and works stably in WSL2 environment.

🚩 Why I Built This
While following a Docker & Laravel course, I wanted to go beyond just following instructions.
I treated this project as my own:

I debugged real issues (timing, permissions)
I iteratively improved the Compose file and container structure
I tested different configurations
I learned to think like someone preparing for real-world Docker deployments

🎯 What's next
Deploying Docker Containers (next labs → will live in /docker-deployment/)

