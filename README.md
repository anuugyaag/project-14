# Project 14: App Deployment using Amazon EKS

## Overview
This project demonstrates deploying a containerized web application on Amazon Elastic Kubernetes Service (EKS) and exposing it publicly using a Kubernetes LoadBalancer service.

## Technologies Used
- Amazon EKS
- Kubernetes
- Docker
- Amazon ECR
- Nginx
- AWS Load Balancer
- Ubuntu

## Project Tasks

1. Provisioned an Amazon EKS cluster.
2. Configured Kubernetes access using `kubectl`.
3. Built a custom Docker image using Nginx.
4. Created an Amazon ECR repository.
5. Pushed the Docker image to Amazon ECR.
6. Deployed the application on the EKS cluster.
7. Exposed the application using a Kubernetes LoadBalancer service.
8. Verified public access to the deployed application.

## EKS Configuration

- **Cluster Name:** `project14-eks`
- **Region:** `eu-north-1`
- **Node Group:** `ng-04df3cf2`
- **Instance Type:** `t3.medium`
- **Replicas:** 2
- **Deployment:** `project14-app`

## ECR Repository

`590507089733.dkr.ecr.eu-north-1.amazonaws.com/project-14-eks-app:latest`

## Public Application URL

[Open Project 14 Application](http://a92a14255a0094509b31a1dba24f4463-1017495999.eu-north-1.elb.amazonaws.com)

## Verification

- EKS cluster status: ACTIVE
- Kubernetes worker node: Ready
- Application pods: 2/2 Running
- Deployment rollout: Successful
- LoadBalancer service: Active
- Public application response: HTTP 200 OK

## Result

Successfully built and deployed a custom Docker application on Amazon EKS and exposed it publicly through an AWS Load Balancer.
