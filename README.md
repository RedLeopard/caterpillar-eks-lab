# Caterpillar EKS Lab
A Terraform-powered Kubernetes cluster for the Caterpillar Architect Interview.


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

## 📂 File Structure


=======
# 🚜 Caterpillar EKS Lab

[![Terraform](https://img.shields.io/badge/Terraform-Cloud-blue?logo=terraform)](https://www.terraform.io/)
[![GitHub Actions](https://img.shields.io/badge/GitHub-Actions-blue?logo=githubactions)](https://github.com/features/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A hands-on cloud project that demonstrates how to deploy a secure, production-ready Amazon EKS cluster using Terraform, GitHub OIDC, and IAM roles. Built for showcasing architecture, DevOps, and cloud engineering skills for the Caterpillar IT Architect interview.

---

## 🌟 Features

- ✅ Deploys an Amazon EKS cluster in `us-east-1`
- ✅ Uses Terraform with GitHub OIDC (no long-lived AWS creds)
- ✅ Creates all networking (VPC, subnets), IAM roles, EKS node groups
- ✅ CI/CD-ready and GitHub Actions compatible
- ✅ Clean Terraform module structure for clarity and reuse

---

## 🏗️ Architecture Overview

```mermaid
graph TD
    GH[GitHub Actions] --> IAM((IAM OIDC Role))
    IAM --> TF[Terraform]
    TF --> EKS((Amazon EKS Cluster))
    EKS --> Nodes[Managed Node Group]


## 📁 File Structure

```text
caterpillar-eks-lab/
├── terraform/
│   ├── main.tf                  # Main infrastructure definitions
│   ├── github-oidc.tf           # IAM OIDC integration with GitHub
│   ├── terraform.tfstate        # Terraform state (usually in .gitignore)
│   └── terraform.tfstate.backup # Terraform state backup
├── README.md                    # Project overview and documentation


>>>>>>> a994974323d9cb7a4b6465f31c56cd6b82d5dd1f
