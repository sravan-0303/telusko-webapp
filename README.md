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


## 📌 Steps

1. **Clone the GitHub Repo**
   - Command: `git clone <repo-url>`
   - ✔️ Output: Local copy of project created.

2. **Create S3 Bucket**
   - Enable Static Website Hosting.
   - Disable Block Public Access if required.
   - ✔️ Output: Bucket created and ready for hosting.

3. **Add S3 Bucket Policy for Public Access**
   - Add JSON policy to allow GET object.
   - ✔️ Output: Website files accessible publicly (only if needed).

4. **Create IAM Roles**
   - Create roles for CodePipeline and CodeBuild.
   - Attach required permissions.
   - ✔️ Output: AWS services have access to S3 and GitHub.

5. **Create CodePipeline**
   - Source: GitHub
   - Build: AWS CodeBuild using `buildspec.yml`
   - Deploy: Amazon S3
   - ✔️ Output: Pipeline created and automation configured.

6. **Configure CodeBuild**
   - Provide environment settings and attach IAM role.
   - ✔️ Output: CodeBuild prepares artifacts for deployment.

7. **Deploy Website via Pipeline**
   - Pipeline runs: Source → Build → Deploy.
   - ✔️ Output: Files automatically uploaded to S3 bucket.

8. **Access Static Website**
   - Use S3 Website Endpoint or CloudFront URL.
   - ✔️ Output: Website successfully hosted.

9. **Make Code Changes and Commit**
   - `git add .`
   - `git commit -m "Updated UI"`
   - `git push origin main`
   - ✔️ Output: New changes automatically built and deployed.

10. **Verify Deployment**
   - Refresh endpoint → See updated version live.
   - ✔️ Output: Application updates without manual upload.

---

## 📌 Final Output

- Static website securely hosted in AWS S3.
- Fully automated CI/CD pipeline built using CodePipeline and CodeBuild.
- Any GitHub commit triggers automatic build and deployment.
- Updates appear instantly on the live hosted website.

---

## 👨‍💻 Author

**SRAVAN**
AWS | CI/CD | DevOps | Cloud Projects
