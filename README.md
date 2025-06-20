# terraform-ansible-spacelift-demo

A hands-on infrastructure automation project using **Terraform** and **Ansible**, orchestrated with **Spacelift**. This setup provisions cloud resources and configures them post-deployment with clean separation between infrastructure and configuration management.

---

## 🚀 Overview

- **Terraform** provisions cloud infrastructure (e.g., EC2, security groups).
- **Ansible** configures the provisioned instances (e.g., install Docker, Nginx).
- **Spacelift** automates and orchestrates the full deployment workflow via stacks and stack dependencies.

---
## ⚡️ Usage

### 1️⃣ Infrastructure with Terraform
```bash
cd tf-ansible-stack-dependencies
terraform init
terraform apply
```
### 2️⃣ Configuration with Ansible
```bash
ansible-playbook -i ansible/inventory ansible/playbooks/site.yml
```
### 3️⃣ Orchestration with Spacelift
- **Terraform Stack:** for infra provisioning
- **Ansible Stack:** configured to run after the Terraform stack
## 🛠️ Technologies
- **Terraform**
- **Ansible**
- **Spacelift**
- **AWS (or any supported cloud)**

---
This is a learning project that demonstrates best practices for integrating Terraform, Ansible, and Spacelift.
