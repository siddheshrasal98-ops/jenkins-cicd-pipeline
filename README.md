# Jenkins CI/CD Pipeline

## Project Overview

This project demonstrates a simple CI/CD pipeline using Jenkins to build and deploy a Dockerized web application.

## Technologies

- Jenkins
- Docker
- Kubernetes
- HTML

## Project Structure

```
jenkins-cicd-pipeline/
│── app/
│   └── index.html
│── Dockerfile
│── Jenkinsfile
│── kubernetes/
│   ├── deployment.yaml
│   └── service.yaml
│── README.md
│── LICENSE
```

## Pipeline Stages

- Checkout Source Code
- Build Docker Image
- Push Docker Image
- Deploy to Kubernetes

## How to Run

Build Docker image

```bash
docker build -t jenkins-demo .
```

Run Docker container

```bash
docker run -d -p 80:80 jenkins-demo
```

Deploy to Kubernetes

```bash
kubectl apply -f kubernetes/
```

## Future Improvements

- Docker Hub integration
- Automated testing
- SonarQube integration
- Trivy security scanning
- Slack notifications
- Blue-Green deployment

## Author

Siddhesh Rasal
