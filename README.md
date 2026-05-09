# AWS ECS Docker Deployment

## Overview

This project demonstrates how to containerize a web application using Docker and prepare it for deployment to Amazon ECS.

The application uses an NGINX container to serve a simple HTML webpage and simulates a real-world container deployment workflow used in DevOps environments.

---

## Technologies Used

- AWS
- Docker
- Amazon ECS
- Amazon ECR
- NGINX
- GitHub
- VS Code

---

## Project Features

- Built a Docker image using a custom Dockerfile
- Containerized a static web application
- Tested the application locally using Docker Desktop
- Exposed the application on port 8080
- Prepared the project for ECS deployment
- Version controlled using Git and GitHub

---

## Project Structure

```bash
aws-ecs-docker-deployment/
│
├── Dockerfile
├── index.html
└── README.md
```

---

## Docker Commands Used

### Build Docker Image

```bash
docker build -t aws-ecs-docker-app .
```

### Run Container

```bash
docker run -d -p 8080:80 --name ecs-docker-test aws-ecs-docker-app
```

### Stop Container

```bash
docker stop ecs-docker-test
```

### Remove Container

```bash
docker rm ecs-docker-test
```

---

## Local Deployment

The application was tested locally using:

```text
http://localhost:8080
```

---

## Future Improvements

- Push Docker image to Amazon ECR
- Deploy application to Amazon ECS Fargate
- Add CI/CD pipeline using GitHub Actions or AWS CodePipeline
- Add CloudWatch logging and monitoring
- Add Terraform automation for ECS infrastructure

---

## Author

Gershon Zormelo  
Cloud & DevOps Engineer