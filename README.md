# catalogue-cd-pipeline
Jenkins CD pipeline for the Catalogue microservice – automates containerization, deployment to Kubernetes, and environment promotion.

# Catalogue Service - CD Pipeline

This repository contains Jenkins pipeline configurations for the **Catalogue Service** Continuous Deployment (CD) process. It automates deployment of the microservice to staging and production environments.

## 🚀 Pipeline Stages
1. **Fetch Artifact** – Download build artifact from Nexus/Artifactory.
2. **Build Docker Image** – Create a Docker image for the service.
3. **Push to Registry** – Upload Docker image to DockerHub/ECR/GCR.
4. **Deploy to Staging** – Deploy the service on Kubernetes/Docker.
5. **Integration Tests** – Run smoke and integration tests.
6. **Deploy to Production** – Controlled promotion to production environment.
7. **Notifications** – Deployment status updates to Slack/Email.
