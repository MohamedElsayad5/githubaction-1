# 🚀 Terraform GitOps CI/CD (GCP + Terraform Cloud)

## 📌 Overview
This project demonstrates a GitOps CI/CD pipeline using Terraform, Terraform Cloud, and GCP.  
Infrastructure is deployed automatically using GitHub pull requests.

---

## 🏗️ Environments
- Dev  
- QA  

Each environment has:
- Separate GCP project  
- Separate Terraform Cloud workspace  

---

## 🔄 Workflow
Feature Branch → Pull Request → Plan → Merge → Apply → Deploy

- PR triggers speculative plan  
- Merge triggers plan + apply  
- Changes are deployed automatically  

---

## 🚀 Promotion
Dev → QA

- Merge to dev → deploy Dev  
- PR from dev to qa → deploy QA  

---

## ☁️ Infrastructure
- Managed Instance Group (MIG)  
- Instance Template  
- Redis (Memorystore)  

---

## 🔐 Variables
- .auto.tfvars → non-sensitive  
- Terraform Cloud → secrets  

---

## 🧹 Resource Removal
❌ Don’t use terraform destroy  
✅ Remove from code → plan → apply  

---

## 🛠️ Tech Stack
- Terraform  
- Terraform Cloud  
- Google Cloud  
- GitHub  

---

## 👨‍💻 Author
Mohamed Mahmoud Mohamed Fayed Elsayed