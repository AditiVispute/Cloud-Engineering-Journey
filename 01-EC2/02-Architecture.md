# ☁️ Amazon EC2 Architecture Overview

## 📌 Introduction

Amazon EC2 (Elastic Compute Cloud) is a scalable virtual server service offered by AWS.

It enables users to deploy applications on virtual machines without managing physical hardware. EC2 architecture integrates compute, networking, storage, and security components to create highly available cloud environments.


---

## 🏗️ Architecture Diagrams

### EC2 Architecture Diagram
![EC2 Architecture](images/ec2-architecture.png)

### AWS Global Infrastructure
![AWS Infrastructure](images/aws-infrastructure.png)

### EC2 Networking Architecture
![EC2 Networking](images/ec2-networking.png)


---

## 🧩 Core Components of EC2 Architecture

### 1️⃣ AWS Region

A Region represents a geographic location containing multiple AWS data centers.

**Advantages:**
- Reduced latency  
- Compliance control  
- Independent fault isolation  


---

### 2️⃣ Availability Zones (AZ)

Availability Zones are isolated data centers within a region.

**Purpose:**
- High availability  
- Disaster recovery  
- Fault tolerance  


---

### 3️⃣ Virtual Private Cloud (VPC)

A VPC is a logically isolated network where EC2 instances run securely.

**Features:**
- Custom IP ranges  
- Route tables  
- Network isolation  


---

### 4️⃣ Subnets

**Public Subnet:**
- Internet accessible  
- Hosts web servers  

**Private Subnet:**
- No direct internet access  
- Hosts databases  


---

### 5️⃣ Internet Gateway

Allows EC2 instances to communicate with the internet.


---

### 6️⃣ EC2 Instance

Virtual machine including:

- CPU  
- Memory  
- Operating system  
- Network interface  


---

### 7️⃣ Amazon Machine Image (AMI)

Preconfigured template used to launch EC2 instances.


---

### 8️⃣ Security Groups

Acts as a virtual firewall controlling inbound and outbound traffic.


---

### 9️⃣ Elastic Block Store (EBS)

Persistent block storage attached to EC2 instances.


---

### 🔟 Elastic Load Balancer (ELB)

Distributes incoming traffic across multiple EC2 instances.


---

### 1️⃣1️⃣ Auto Scaling

Automatically increases or decreases instances based on traffic demand.


---

## 🔄 EC2 Architecture Workflow

1. User launches EC2 instance using AMI  
2. Instance is deployed inside VPC  
3. Security groups manage traffic rules  
4. EBS storage is attached  
5. Load balancer distributes traffic  
6. Auto Scaling maintains performance  


---

## ⚡ High Availability Design

Best practices include:

- Multi-Availability Zone deployment  
- Load balancing  
- Auto Scaling groups  
- Snapshot backups  


---

## 🚀 Advantages of EC2 Architecture

- Elastic scalability  
- Secure networking  
- Cost efficiency  
- High reliability  
- Global deployment support  


---

## 📌 Conclusion

Amazon EC2 architecture combines computing power, storage, networking, and security into a flexible cloud platform.

It enables organizations to deploy scalable and fault-tolerant applications efficiently.
