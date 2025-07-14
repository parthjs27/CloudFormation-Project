# ☁️ AWS CloudFormation - Static Website on EC2 in VPC

This project uses **AWS CloudFormation** to deploy a static website hosted on an **EC2 instance** inside a **custom VPC**. The EC2 instance automatically clones a static site from a GitHub repository and serves it via Apache.

---

## 📌 Features

- Custom **VPC** with public subnet
- **Internet Gateway** and route configuration
- **Security Group** allowing HTTP and SSH access
- **EC2 instance** (Amazon Linux 2, `t2.micro`)
- **Apache web server** setup
- **Git clone** of static site from this GitHub repo
- Automatic deployment via **CloudFormation YAML**

---

## 🧱 Project Structure
```bash
    CloudFormation-Project/
    │
    ├── mysite/                   # Static website source
    │   ├── assets/
    │   ├── index.html
    │   └── readme.txt
    │
    ├── output_images/           # Screenshots or diagrams
    │   └── architecture-diagram.png
    │
    ├── static_hosting.yaml      # CloudFormation template
    ├── README.md                # Project documentation

```

![Architecture Diagram](./assets/architecture-diagram.png)

---

## 🔧 Prerequisites

- An AWS account
- An EC2 Key Pair (`.pem`) in the region you're deploying
- Your GitHub static site stored in the `mysite/` folder of this repo (✅ already done!)

---

## 🚀 How to Deploy

1. Clone this repo:
   ```bash
   git clone https://github.com/parthjs27/CloudFormation-Project.git
   cd CloudFormation-Project
