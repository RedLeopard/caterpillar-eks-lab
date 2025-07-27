# Caterpillar EKS Lab

This project showcases the deployment of a secure and production-grade Amazon EKS (Elastic Kubernetes Service) cluster using Terraform. It was designed as part of a portfolio project for a Staff IT Architect interview with Caterpillar.

---

## 📌 Project Overview

- **Infrastructure as Code**: Provisioned entirely using Terraform
- **Cloud Platform**: Amazon Web Services (AWS)
- **Kubernetes**: Amazon EKS with managed node groups
- **CI/CD Integration**: OIDC authentication for GitHub Actions
- **Security Best Practices**: Minimal permissions, separate IAM roles
- **Region**: `us-east-1`

---

## 🏗️ Features

- ✅ **EKS Cluster Deployment** (via `aws_eks_cluster`)
- ✅ **Managed Node Group**
- ✅ **OIDC IAM Role for GitHub Actions**
- ✅ **Public Subnets across AZs**
- ✅ **Modular, Readable Terraform Code**

---

## 📁 File Structure

```text
caterpillar-eks-lab/
├── terraform/
│   ├── main.tf                  # Main infrastructure definitions
│   ├── github-oidc.tf           # IAM OIDC integration with GitHub
│   ├── terraform.tfstate        # Terraform state (usually in .gitignore)
│   └── terraform.tfstate.backup # Terraform state backup
├── README.md                    # Project overview and documentation

