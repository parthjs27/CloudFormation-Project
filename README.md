# ☁️ AWS CloudFormation - Static Website on EC2 in VPC

This project uses **AWS CloudFormation** to deploy a static website hosted on an **EC2 instance** inside a **custom VPC**. The EC2 instance automatically clones a static site from a GitHub repository and serves it via Apache.

---

## 📌 Features

- Custom **VPC** with public subnet
- **Internet Gateway** and route configuration
- **Security Group** allowing HTTP and SSH access
- **EC2 instance** (Ubuntu 22.04 LTS, `t2.micro`)
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
    │
    ├── static_hosting.yaml      # CloudFormation template
    ├── README.md                # Project documentation

```
### Project Output
![Website](output_images/1.png)

---

## 🔧 Prerequisites

- An AWS account
- An EC2 Key Pair (`.pem`) in the region you're deploying
- Prior knowledge about YAML
---