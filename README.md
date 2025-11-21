# 🔐 Secure AWS CI/CD Pipeline for Static Web Application

This mini project demonstrates building a **secure CI/CD pipeline** using AWS services to host and automatically deploy a static website. The pipeline ensures automated updates whenever the GitHub repository receives a new commit.

---

## 🚀 Architecture Overview

AWS Services Used:

- **Amazon S3** → Static Website Hosting  
- **IAM** → Secure role and permissions  
- **AWS CodePipeline** → CI/CD Orchestration  
- **AWS CodeBuild** → Build and deployment automation  
- **CloudFront (optional)** → Secure CDN distribution  
- **GitHub** → Source Control Repository  

---

## 🧰 Prerequisites

- AWS Account
- GitHub Repository with static website files (`index.html`, assets, etc.)
- `buildspec.yml` file in your repository
- AWS IAM role with required permissions

---


git clone <your-github-repo-url>
cd <project-folder>
