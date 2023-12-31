# AWS EKS Deployment of Real-Time 2048 Game Using Fargate

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Process Overview](#process-overview)
   - 3.1 [Setting Up EKS with Fargate](#setting-up-eks-with-fargate)
   - 3.2 [Configuring IAM and OIDC](#configuring-iam-and-oidc)
   - 3.3 [Implementing ALB Ingress Controller](#implementing-alb-ingress-controller)
   - 3.4 [Deploying the 2048 Game Application](#deploying-the-2048-game-application)
   - 3.5 [Sample App Deployment](#sample-app-deployment)
4. [Conclusion](#conclusion)

## Introduction

This project showcases deploying a real-time 2048 game application on Amazon Elastic Kubernetes Service (AWS EKS) using AWS Fargate. It's an exemplary demonstration of cloud-native application deployment and management, emphasizing Kubernetes orchestration, AWS services, and modern DevOps practices.

## Prerequisites

To begin, ensure you have the following tools installed and configured:
- **kubectl**: Essential for interacting with Kubernetes clusters.
- **eksctl**: Streamlines working with EKS clusters, automating many tasks.
- **AWS CLI**: A critical tool for interacting with AWS services.

## Process Overview

### Setting Up EKS with Fargate

The project starts by establishing an EKS cluster optimized for serverless deployment using AWS Fargate. Fargate allows running Kubernetes pods without managing EC2 instances, simplifying the operational aspect.

### Configuring IAM and OIDC

A key step is setting up IAM roles and Identity Providers (OIDC) for the EKS cluster. This configuration is crucial for managing permissions and ensuring secure communication between AWS services and the Kubernetes cluster.

### Implementing ALB Ingress Controller

To expose the 2048 game application externally, an ALB Ingress Controller is deployed. This involves creating an IAM policy, setting up an IAM role, and deploying the ALB controller using Helm charts. The ALB Ingress Controller manages traffic routing and provides an efficient way to expose Kubernetes services.

### Deploying the 2048 Game Application

The deployment process includes creating a Fargate profile and deploying the game's Kubernetes resources such as deployments, services, and ingress resources. This setup demonstrates the application's deployment in a Kubernetes-managed environment.

### Sample App Deployment

Additionally, the project encompasses deploying a sample Linux-based application, demonstrating the ability to manage and deploy diverse workloads on EKS.

## Conclusion

This project highlights key aspects of deploying and managing applications on AWS EKS using Fargate and the AWS Load Balancer Controller. It underscores the integration of cloud-native technologies with Kubernetes, emphasizing scalability, ease of management, and operational efficiency in a DevOps environment.
