# 🚀 AWS Terraform Infrastructure - Scalable & Cost-Optimized Deployment

## 📌 Overview
This project provides a **production-grade AWS infrastructure** using **Terraform**. It integrates **networking, compute, serverless, storage, monitoring, and cost optimization strategies** in a **multi-region disaster recovery setup**.  

## 🎯 **Key Features**
✅ **Infrastructure as Code (IaC)** using **Terraform**  
✅ **High Availability & Auto Scaling** (VPC, ALB, ASG, EC2, RDS, EKS)  
✅ **Serverless API & Data Storage** (AWS Lambda, API Gateway, DynamoDB)  
✅ **Multi-Region Disaster Recovery** (Route 53 failover, S3 Replication)  
✅ **Security Best Practices** (IAM Roles, Security Groups, Private Subnets)  
✅ **Monitoring & Logging** (CloudWatch, Datadog)  
✅ **CI/CD Deployment** (GitHub Actions, Terraform Cloud)  
✅ **Cost Optimization Strategies** (Spot Instances, Savings Plans, S3 Lifecycle)  

---

## 🏗 **Architecture Diagram**
![Architecture Diagram](docs/architecture-diagram.png)  

---

## 📂 **Project Structure**
```bash
aws-terraform-project/
│── README.md            # Project Overview
│── LICENSE              # Open-source license
│── .gitignore           # Ignore Terraform state, AWS credentials
│
├── terraform/           # Terraform Configuration
│   ├── modules/         # Reusable Terraform Modules
│   │   ├── vpc/  
│   │   ├── ec2/  
│   │   ├── rds/  
│   │   ├── eks/  
│   │   ├── s3/  
│   │   ├── lambda/  
│   │   ├── alb/  
│   │   ├── route53/  
│   ├── main.tf          # Main Terraform configuration
│   ├── variables.tf     # Input variables
│   ├── outputs.tf       # Output variables
│   ├── backend.tf       # Terraform backend (S3 + DynamoDB)
│   ├── terraform.tfvars # Environment-specific variables
│
├── serverless/          # Serverless App (Lambda + API Gateway)
│   ├── lambda-functions/
│   │   ├── function1/
│   │   ├── function2/
│   ├── api-gateway-config/
│
├── eks-microservices/   # Microservices deployed on EKS
│   ├── service1/
│   ├── service2/
│   ├── k8s-manifests/   # Kubernetes YAML files
│
├── monitoring/          # CloudWatch & Datadog Setup
├── ci-cd/               # GitHub Actions, Terraform Cloud, Jenkins Pipelines
└── docs/                # Documentation & Diagrams
