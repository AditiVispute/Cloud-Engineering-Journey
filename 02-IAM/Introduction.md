# 🔐 AWS IAM (Identity and Access Management)

---

## 📌 Introduction

**AWS Identity and Access Management (IAM)** is a foundational security service provided by **Amazon Web Services (AWS)** that enables you to securely manage access to AWS resources.

<img width="1200" height="628" alt="iam1" src="https://github.com/user-attachments/assets/f4707009-bf33-4b45-ab23-9de9c3cb9374" />

IAM allows organizations to control:

- **Who** can access AWS resources  
- **What** actions they can perform  
- **Which** resources they can use  
- **When** and **how** access is granted  

👉 It acts as the **security gatekeeper** of an AWS environment.

👉 IAM is a **global service**, meaning configurations apply across all AWS regions.

---

## 🧠 IAM Concept Overview

AWS IAM works by verifying identities and enforcing permissions through policies.

Every request made to AWS services must pass:

- Authentication (Who are you?)  
- Authorization (What can you do?)  

---

## ❓ Why AWS IAM is Important

Cloud environments host sensitive applications and data. Without controlled access, systems become vulnerable.

IAM provides:

- Secure authentication  
- Fine-grained authorization  
- Centralized permission management  
- Protection against unauthorized access  

👉 IAM follows the **Principle of Least Privilege**, meaning users get only the permissions they need.

---

## 🧩 Core Components of IAM

---

### 👤 IAM Users

An IAM User represents an individual person or application interacting with AWS.

**Features:**
- Unique username  
- Login password or access keys  
- Assigned permissions  

**Examples:**
- Developer  
- Administrator  
- Application service account  

---

### 👥 IAM Groups

IAM Groups organize users with similar responsibilities.

Instead of assigning permissions individually:
- Assign policies to groups  
- Add users to groups  

**Examples:**
- Developers  
- DevOps Team  
- ReadOnly Users  

---

### 🔄 IAM Roles

IAM Roles provide **temporary permissions**.

**Used when:**
- AWS services need access to other services  
- Applications require temporary credentials  
- Cross-account access is required  

**Examples:**
- EC2 accessing S3  
- Lambda writing logs to CloudWatch  

---

### 📜 IAM Policies

Policies define permissions using JSON documents.

**Example Policy:**

```json
{
  "Effect": "Allow",
  "Action": "s3:ListBucket",
  "Resource": "*"
}
