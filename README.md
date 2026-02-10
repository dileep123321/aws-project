# Python App Deployment on AWS EKS using GitHub Actions

## Project Purpose
This repository demonstrates an end-to-end CI/CD pipeline that deploys a containerized Python application to AWS EKS using GitHub Actions and Amazon ECR.

## Workflow Trigger
The GitHub Actions workflow is triggered on push to the main branch or manually from GitHub Actions UI.

## Automatic Trigger
git add .
git commit -m "Update application"
git push origin main

## Manual Trigger
1. Open GitHub repository
2. Go to Actions
3. Select CI/CD Pipeline – Deploy Python App to AWS EKS
4. Click Run workflow

## Verify Deployment
kubectl get pods
kubectl get svc python-app-service

## Cleanup
eksctl delete cluster --name demo-eks --region us-east-1

