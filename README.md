# Iron Man Landing Page — Docker Deployment

A practical containerization project demonstrating how to package and serve a custom Iron Man landing page using Docker and Nginx on AWS EC2.

## 🚀 Project Overview

The website was packaged into a custom Docker image and deployed inside an Nginx container on an AWS EC2 Linux server.

## 🛠️ Technologies Used

- AWS EC2
- Docker
- Docker Hub workflow
- Nginx
- HTML and CSS
- Linux

## 🏗️ Deployment Architecture

```text
Browser
   |
   v
AWS EC2 — Port 9090
   |
   v
Docker Container: netflix-web
   |
   v
Nginx — Port 80
   |
   v
Custom Iron Man Landing Page
```

**Port mapping:** Host port `9090` → Container port `80`

## ⚙️ Key Implementation Steps

1. Prepare the Linux server and install Docker.
2. Pull and inspect Docker images.
3. Create the custom website using HTML and CSS.
4. Write a Dockerfile based on Nginx.
5. Build the image using `docker build -t netflix:v1 .`.
6. Run the container using `docker run -d --name netflix-web -p 9090:80 netflix:v1`.
7. Verify the deployment through a browser.
8. Explore Docker networking, volumes, troubleshooting, and Docker Hub publishing workflow.

## 📄 Project Documentation

The accompanying PDF contains the implementation guide, commands, troubleshooting steps, and screenshots.

**Documentation:** `Iron-Man-Docker-Deployment-Documentation.pdf`

## 📚 Skills Demonstrated

- Docker image and container management
- Dockerfile creation
- Nginx website hosting
- AWS EC2 deployment
- Port mapping and troubleshooting
- Docker networking and volumes

## 🔐 Security Notes

Use restrictive AWS security-group rules and avoid exposing administrative ports to the public internet. Never commit credentials, private keys, or access tokens.

---

**Project Category:** Cloud Computing & Containerization
