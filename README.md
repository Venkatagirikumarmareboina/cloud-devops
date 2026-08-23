# Cloud DevOps CI/CD Project

A hands-on Cloud DevOps project demonstrating how a web application can be containerized, tested, published, and deployed to AWS.

## 🚀 Project Architecture

GitHub → GitHub Actions → Docker → Docker Hub → AWS EC2 → Live Web Application

## 🛠️ Technologies Used

- Git & GitHub
- Docker
- Nginx
- GitHub Actions
- Docker Hub
- AWS EC2
- Ubuntu Linux

## 🔄 CI/CD Workflow

1. Source code is maintained in GitHub.
2. GitHub Actions automatically runs when changes are pushed to `main`.
3. Docker builds the application image.
4. The image is tested in the CI workflow.
5. GitHub Actions securely logs in to Docker Hub using GitHub Secrets.
6. The Docker image is pushed to Docker Hub.
7. The image is pulled onto an AWS EC2 Ubuntu server.
8. The application runs inside a Docker container.
9. Port 80 exposes the application to the internet.

## 🐳 Docker

Docker is used to package the web application into a portable container.

Docker image:

`venkatagirikumarmareboina/cloud-devops-web:latest`

## ☁️ AWS Deployment

The application is deployed on an AWS EC2 Ubuntu server.

The Docker container is exposed through port 80 and can be accessed through the EC2 public IPv4 address.

## 🔐 Security

GitHub Actions uses repository secrets for Docker Hub authentication.

SSH access to the EC2 server is restricted to the configured IP address, while HTTP port 80 is publicly accessible for the web application.

## 📚 What I Learned

- Version control with Git and GitHub
- Docker image and container management
- Writing and using a Dockerfile
- CI automation with GitHub Actions
- Secure secret management
- Publishing Docker images to Docker Hub
- Deploying containers to AWS EC2
- Connecting to Linux servers using SSH
- Exposing a containerized application to the internet

## 🎯 Project Goal

The goal of this project is to build practical Cloud DevOps skills by taking an application from source code to a publicly accessible cloud deployment.
