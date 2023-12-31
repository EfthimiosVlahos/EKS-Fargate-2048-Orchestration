# AWS EKS Deployment of Real-Time 2048 Game Using Fargate

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Process Overview](#process-overview)
   - 3.1 [Setting Up EKS with Fargate](#setting-up-eks-with-fargate)
   - 3.2 [Configuring IAM and OIDC](#configuring-iam-and-oidc)
   - 3.3 [Implementing ALB Ingress Controller](#implementing-alb-ingress-controller)
   - 3.4 [Deploying the 2048 Game Application](#deploying-the-2048-game-application)
4. [Conclusion](#conclusion)

# AWS EKS Deployment of Real-Time 2048 Game Using Fargate

## Introduction

This project focuses on deploying a real-time 2048 game application utilizing Amazon Elastic Kubernetes Service (AWS EKS) and AWS Fargate. It serves as a prime example of deploying cloud-native applications, showcasing how Kubernetes can be orchestrated on AWS to manage and scale applications efficiently. The project leverages the power of AWS services combined with modern DevOps practices to create a scalable, resilient, and efficient deployment.

## Prerequisites

Before starting, it's essential to have the following tools ready:

- **kubectl**: The command-line tool for Kubernetes, allowing you to run commands against Kubernetes clusters. It's crucial for deploying and managing applications, inspecting cluster resources, and viewing logs.
  
- **eksctl**: A simple CLI tool for creating clusters on EKS. It simplifies the process of creating and managing clusters, abstracting away much of the complexity of managing Kubernetes.
  
- **AWS CLI**: The command-line tool for AWS, providing direct access to AWS services. It's used to manage AWS resources, automate scripts, and interact with AWS services like EKS and Fargate.

## Process Overview

### Setting Up EKS with Fargate

The project begins by setting up an EKS cluster, opting for AWS Fargate as the compute engine. Fargate's serverless compute engine allows for running Kubernetes pods without managing EC2 instances, thus simplifying operations and reducing the overhead of cluster management.

### Configuring IAM and OIDC

Configuring IAM roles and setting up an OIDC (OpenID Connect) provider are crucial for secure and efficient management of permissions within your EKS cluster. This step ensures that the cluster has the necessary permissions to interact with other AWS services securely and efficiently, aligning with best practices for security and access management.

### Implementing ALB Ingress Controller

Deploying the ALB (Application Load Balancer) Ingress Controller is a pivotal step in exposing the 2048 game application to the external network. This process involves creating an IAM policy, configuring an IAM role for the ALB Ingress Controller, and utilizing Helm charts for deployment. The ALB Ingress Controller facilitates efficient traffic management, enabling scalable and secure access to the application.

### Deploying the 2048 Game Application

This phase includes the deployment of the 2048 game using Kubernetes resources managed by AWS Fargate. A Fargate profile is created for the game deployment, followed by the setup of necessary Kubernetes resources such as Deployments, Services, and Ingress. This demonstrates deploying and managing a real-time application in a cloud-native environment effectively.


## Conclusion

Overall, this project effectively demonstrates the deployment and management of applications on AWS EKS using Fargate and the AWS Load Balancer Controller. It highlights the synergy between cloud-native technologies and Kubernetes, focusing on scalability, ease of management, and the efficiency of DevOps processes, providing a valuable example of modern application deployment strategies.




https://github.com/EfthimiosVlahos/EKS-Fargate-2048-Orchestration/assets/56899588/4064236a-e2eb-4044-af45-02774709ef64

