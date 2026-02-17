# Terraform AWS Infrastructure Setup

This project demonstrates how to deploy a basic infrastructure.  
The setup includes a custom VPC, subnet, security group, and an EC2 instance hosting a simple static website (`index.html`).

---

## 🚀 Project Overview

This project is designed to show how cloud resources can be provisioned automatically using Terraform.  
It’s useful for learning, interviews, and demonstrating IaC (Infrastructure as Code) skills.

### **What this project creates**
- A Virtual Private Cloud (VPC)
- A public subnet
- Route table + Internet Gateway for public access
- Security group allowing HTTP access
- EC2 instance
- Simple static webpage (`index.html`) hosted on the instance

---

## 🛠️ Technologies Used

- **Terraform** (Infrastructure as Code)
- **AWS EC2** (Compute)
- **AWS VPC** (Networking)
- **HTML** (Static website)

---

## 📂 Project Structure

.
├── index.html # Static webpage
├── main.tf # Main Terraform configuration
├── provider.tf # Provider configuration
└── README.md # Project documentation


---

## ✔️ Prerequisites

Make sure you have:

- Terraform installed
- AWS CLI configured with valid credentials
- An AWS account
- Basic understanding of EC2 + VPC

---

## 🧩 How to Use This Project

### **1. Initialize Terraform**
terraform init


### **2. Validate configuration**
terraform validate


### **3. Preview the infrastructure**
terraform plan


### **4. Deploy the infrastructure**
terraform apply -auto-approve


### **5. Access Your Website**
Terraform will output the EC2 instance public IP.  
Open it in your browser:

http://<EC2-PUBLIC-IP>


---

## 🧹 Destroying the Infrastructure (Cleanup)

If you want to remove everything:

terraform destroy -auto-approve


---

## 🎯 Purpose of This Project

- Demonstrate Terraform skills  
- Show understanding of AWS networking & EC2  
- Provide a clean IaC example for interviews and GitHub portfolio  
- Simple and easy for HR/Recruiters to understand

---

## 📌 Future Enhancements (Optional)

- Add S3 static website hosting  
- Add load balancer  
- Add modular Terraform structure  
- Add CI/CD pipeline  
