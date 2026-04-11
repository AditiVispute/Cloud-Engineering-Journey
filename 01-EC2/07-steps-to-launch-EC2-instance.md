# ☁️ Steps to Launch an EC2 Instance

---

## 📌 Introduction

An **EC2 Instance** is a virtual server in the cloud provided by **Amazon Web Services (AWS)**.

Launching an EC2 instance allows you to:
- Run applications  
- Host websites  
- Deploy databases  
- Build scalable infrastructure  

👉 Without owning physical hardware.

---

## 🖼️ EC2 Launch Workflow Diagram

<img width="1536" height="1024" alt="l1" src="https://github.com/user-attachments/assets/b86551bd-a557-4145-8f0d-dcea404aaee4" />


---

## 🚀 Step-by-Step Guide to Launch EC2 Instance

---

### 🔹 Step 1 — Login to AWS Console

1. Open AWS Management Console  
2. Search **EC2** in the services search bar  
3. Click **EC2 Dashboard**  

---

## 🖥️ EC2 Dashboard

<img width="1920" height="909" alt="l2" src="https://github.com/user-attachments/assets/5d765399-6bac-4078-ba52-20c0213249da" />


---

### 🔹 Step 2 — Click Launch Instance

- Select **Instances**  
- Click **Launch Instance**  

---

## 🚀 Launch Instance Page

<img src="https://github.com/user-attachments/assets/b776cd20-6c96-46c5-94c7-5946db07d28a" width="900"/>

---

### 🔹 Step 3 — Choose Amazon Machine Image (AMI)

AMI contains:

- Operating System  
- Preinstalled software  
- Configuration settings  

**Examples:**
- Amazon Linux  
- Ubuntu  
- Windows Server  

---

### 🔹 Step 4 — Choose Instance Type

Instance type defines:

- CPU  
- Memory  
- Performance  

**Example:**

| Instance Type | Use Case             |
|---------------|----------------------|
| t2.micro      | Free tier testing    |
| t3.medium     | Applications         |
| m5.large      | Production workloads |

---

## ⚙️ Instance Type Selection

<img width="1920" height="910" alt="l4" src="https://github.com/user-attachments/assets/758c6934-9aba-4f44-8cb4-8ba542fe6cb6" />



---

### 🔹 Step 5 — Configure Instance Details

Configure:

- Number of instances  
- Network (VPC)  
- Subnet  
- Auto-assign Public IP  

---

### 🔹 Step 6 — Add Storage

Attach storage using **EBS Volume**.

**Example:**
- 8 GB (Free Tier)  
- SSD or HDD storage  

---

## 💾 Storage Configuration

<img width="1920" height="907" alt="l5" src="https://github.com/user-attachments/assets/cb835f74-a794-4b28-b785-b537b1608121" />



---

### 🔹 Step 7 — Add Tags

Tags help organize resources.

**Example:**
Name = My-Server
Environment = Dev


---

### 🔹 Step 8 — Configure Security Group

Acts as a firewall.

**Common Rules:**

| Protocol | Port | Purpose        |
|----------|------|----------------|
| SSH      | 22   | Linux Access   |
| HTTP     | 80   | Website        |
| HTTPS    | 443  | Secure Website |

---

## 🔐 Security Group Configuration

<img width="1920" height="910" alt="l6" src="https://github.com/user-attachments/assets/53ee281c-abb7-4304-936e-e21d39b81cc6" />


---

### 🔹 Step 9 — Create Key Pair

Key Pair is required for secure login.

- Download `.pem` file  
- Keep it safe  

---

## 🔑 Key Pair Creation

<img width="1920" height="907" alt="l7" src="https://github.com/user-attachments/assets/a6a88124-99da-4096-85bd-b0c2ad112ddd" />


---

### 🔹 Step 10 — Launch Instance

👉 Click **Launch Instance**

Your EC2 server will start within seconds.

---

## 🟢 Instance Running State

<img width="1920" height="907" alt="l8" src="https://github.com/user-attachments/assets/1eac2fb0-097f-4f8c-80ec-c82a2f4c7428" />


---

## 🔄 EC2 Instance Lifecycle

Launch → Pending → Running → Stopping → Stopped → Terminated


---

## 🎯 Result

After launching, you can:

- Connect using SSH  
- Deploy web applications  
- Install software  
- Host websites  
- Run cloud projects  
