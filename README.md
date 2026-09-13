# AWS VPC Infrastructure with Terraform

## 📌 Project Overview

This project demonstrates the design and deployment of **AWS VPC infrastructure using Terraform (Infrastructure as Code)**.

The project creates a structured AWS network environment with public and private subnets, Internet Gateway, NAT Gateway, route tables, security groups, and an EC2 instance.

The complete infrastructure is provisioned and managed using Terraform.

---

## 🎯 Project Purpose

The main purpose of this project is to gain practical experience in:

* AWS networking
* Terraform Infrastructure as Code (IaC)
* Public and private subnet architecture
* Secure cloud infrastructure design
* EC2 deployment
* NAT Gateway and Internet Gateway configuration
* Terraform infrastructure lifecycle management

---

## ✨ Features

* Custom AWS VPC configuration
* Public and private subnet architecture
* Internet Gateway for public internet connectivity
* NAT Gateway for private subnet outbound access
* Public and private route tables
* Security Group configuration
* EC2 instance deployment
* Infrastructure managed completely through Terraform
* Reproducible and version-controlled infrastructure
* Terraform validation, planning, deployment, and destruction

---

## 🛠️ Tools & Technologies

| Technology           | Purpose                        |
| -------------------- | ------------------------------ |
| **AWS**              | Cloud Infrastructure           |
| **Terraform**        | Infrastructure as Code         |
| **VPC**              | Network Architecture           |
| **EC2**              | Compute                        |
| **NAT Gateway**      | Private Subnet Internet Access |
| **Internet Gateway** | Public Internet Access         |
| **Route Tables**     | Network Traffic Routing        |
| **Security Groups**  | Network Security               |
| **Linux**            | Server Administration          |
| **Git & GitHub**     | Version Control                |

---

## 🏗️ AWS Infrastructure

### VPC

* CIDR: `10.0.0.0/16`

### Public Subnet

* CIDR: `10.0.0.0/22`
* Internet Gateway connectivity
* NAT Gateway deployed here

### Private Subnet

* CIDR: `10.0.4.0/22`
* Outbound internet access through NAT Gateway
* EC2 instance deployed here

### Security Group

Configured for:

* SSH — Port `22`
* HTTP — Port `80`
* Outbound traffic

---

## 📂 Repository Structure

```text
terraform-aws-vpc/
│
├── main.tf
├── nat.tf
├── security.tf
├── privtinst.tf
├── keypair.pub
├── .gitignore
└── README.md
```

### File Description

* `main.tf` — VPC, subnet, Internet Gateway and route table configuration
* `nat.tf` — Elastic IP and NAT Gateway configuration
* `security.tf` — Security Group configuration
* `privtinst.tf` — Private EC2 instance configuration
* `keypair.pub` — Public SSH key
* `.gitignore` — Prevents sensitive Terraform and key files from being committed
* `README.md` — Project documentation

> ⚠️ **Security:** Never commit private SSH keys, AWS credentials, `.terraform/`, or Terraform state files to GitHub.

---

## 🔄 Terraform Workflow

```text
Terraform Configuration
          ↓
    terraform init
          ↓
   terraform validate
          ↓
     terraform plan
          ↓
     terraform apply
          ↓
    AWS Infrastructure
          ↓
    terraform destroy
```

---

## 🚀 Terraform Commands

### Initialize

```bash
terraform init
```

### Validate

```bash
terraform validate
```

### Review Infrastructure

```bash
terraform plan
```

### Create Infrastructure

```bash
terraform apply
```

### Destroy Infrastructure

```bash
terraform destroy
```

---

## 🎓 Key Learning Outcomes

Through this project, I gained practical experience with:

* AWS VPC networking
* Public vs private subnet architecture
* Internet Gateway and NAT Gateway
* Route table configuration
* Security Group configuration
* EC2 deployment
* Terraform Infrastructure as Code
* Terraform lifecycle management
* Linux-based cloud administration
* Git and GitHub version control

---

## 📈 Future Improvements

Planned improvements include:

* Multi-AZ architecture
* Multiple public and private subnets
* Application Load Balancer
* Auto Scaling Group
* Terraform variables and outputs
* Terraform modules
* Remote state using Amazon S3
* State locking
* CloudWatch monitoring
* GitHub Actions CI/CD

---

## 👨‍💻 Author

**Sumanth PS Yadav**

**Aspiring DevOps Engineer**

### Skills

`AWS` • `Linux` • `Docker` • `Terraform` • `Ansible` • `Git`

---

## ⭐ Project Goal

This project is part of my **hands-on DevOps and Cloud learning journey**, focused on building real-world AWS infrastructure using automation and Infrastructure as Code.
