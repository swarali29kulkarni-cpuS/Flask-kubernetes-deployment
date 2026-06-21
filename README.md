# Flask Kubernetes Deployment

A cloud-native Flask web application deployed using Docker and Kubernetes.

## Project Overview

This project demonstrates containerization and orchestration of a Python Flask application using Docker and Kubernetes. The application is deployed on a local Kubernetes cluster created with Minikube and exposed through a Kubernetes Service.

## Features

- Docker containerization
- Kubernetes Deployment
- Kubernetes Service
- Replica management
- Horizontal scaling
- Minikube local cluster

## Tech Stack

- Python
- Flask
- Docker
- Kubernetes
- Minikube
- YAML
- GitHub

## Project Structure

```text
app.py
requirements.txt
Dockerfile
deployment.yaml
service.yaml
README.md
```

## Build Docker Image

```bash
docker build -t flask-k8s-app .
```

## Load Image into Minikube

```bash
minikube image load flask-k8s-app
```

## Deploy Application

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

## Verify Deployment

```bash
kubectl get pods
kubectl get deployments
```

## Scale Application

```bash
kubectl scale deployment flask-app --replicas=5
```

## Output

The application was successfully deployed on Kubernetes and accessed through a Kubernetes Service.

Output:

Hello from Kubernetes!

## Learning Outcomes

- Containerized applications using Docker
- Created Kubernetes Deployments and Services
- Managed Pods and Replicas
- Performed horizontal scaling
- Worked with Minikube and kubectl
- Understood cloud-native application deployment
