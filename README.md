# 🚀 EC2 Static Website Deployment with GitHub Actions + Docker

This project demonstrates how to **automatically build and deploy a static website** on an **AWS EC2 instance** using **GitHub Actions** and **Docker**. When you push code to GitHub, the CI/CD workflow builds a Docker image, pushes it to Docker Hub, and runs it on your EC2 instance to serve your website.

---

## 📦 Stack Used

- 🐳 Docker
- 🖥️ AWS EC2 (Ubuntu)
- 🔁 GitHub Actions
- 🌐 NGINX or Apache (inside container)

---

## 🔄 Workflow Overview

### Step 1: Create GitHub Repository

Push your static files (`index.html`, `css`, etc.) and Dockerfile to a new GitHub repository.

### Step 2: Add GitHub Actions Workflow

In `.github/workflows/deploy.yml`, define a GitHub Action that:

- Builds the Docker image
- Pushes it to Docker Hub
- SSHs into the EC2 instance
- Pulls and runs the container
