# TASK-3-Infrastructure-as-Code-IaC-with-Terraform


## 📌 Project Overview

This project demonstrates Infrastructure as Code (IaC) using Terraform to provision a local Docker container automatically.

Instead of manually running Docker commands, the infrastructure is created, managed, and destroyed using Terraform configuration files.

This task is part of the DevOps Internship Program.

---

## 🎯 Objective

Provision a local Docker container using Terraform.

---

## 🛠️ Tools & Technologies Used

- Terraform
- Docker
- Git
- GitHub
- Ubuntu (Linux Environment)

---

## 📚 What is Infrastructure as Code (IaC)?

Infrastructure as Code (IaC) is the process of managing and provisioning infrastructure through code instead of manual processes.

Benefits:
- Automation
- Version control
- Reusability
- Faster deployment
- Consistency

---

## 📂 Project Structure

``

terraform-docker-project/
│
├── main.tf
├── README.md

``

--

## 📝 Terraform Configuration (main.tf)

The Terraform file performs the following:

1. Configures Docker provider
2. Pulls nginx image from Docker Hub
3. Creates a Docker container
4. Maps port 80 (container) to port 8080 (local machine)

---

## ⚙️ Steps Performed

### 1️⃣ Initialize Terraform

```

terraform init

```

Downloads required Docker provider plugin.

---

### 2️⃣ Check Execution Plan

```

terraform plan

```

Shows what resources Terraform will create.

---

### 3️⃣ Apply Configuration

```

terraform apply

```

Creates:
- Docker Image (nginx)
- Docker Container

---

### 4️⃣ Verify Container

```

docker ps

```

Then open in browser:

```

[http://localhost:8080](http://localhost:8080)

```

Nginx welcome page is displayed.

---

### 5️⃣ Destroy Infrastructure

```

terraform destroy

```

Removes:
- Docker container
- Docker image

---

## 📦 Terraform Workflow

```

Write Code → terraform init → terraform plan → terraform apply → terraform destroy

```

---

## 📁 Important Files

### main.tf
Contains Terraform configuration to:
- Define provider
- Create Docker image
- Create Docker container

### .gitignore
Prevents sensitive and unnecessary files from being pushed to GitHub:

``

.terraform/
terraform.tfstate
terraform.tfstate.backup

``

--




Tell me what you want next 💪
