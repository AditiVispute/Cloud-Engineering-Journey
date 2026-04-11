
# ☁️ Amazon EC2 Instance Lifecycle

An **EC2 Instance Lifecycle** describes the different states an instance goes through — from creation to termination — inside **Amazon Web Services (AWS)**.

Understanding lifecycle states helps you:

- Manage servers efficiently  
- Reduce AWS costs  
- Control application availability  
- Avoid accidental data loss  

---

## 🖼️ EC2 Instance Lifecycle Diagram

![cycle 1](https://github.com/user-attachments/assets/92da3981-31ec-4e7f-81f1-672dbf4d3ea4)

---

## 🔄 EC2 Lifecycle States

---

### 1️⃣ Pending State

**What happens:**
- Instance is launching  
- AWS allocates resources (CPU, RAM, Network)  
- Operating system boots  

👉 Instance is **not yet usable**

**Billing:** No charges  

---

### 2️⃣ Running State

**What happens:**
- Instance becomes active  
- Applications start running  
- Users can connect via SSH/RDP  

👉 This is the **working state**

**Billing:** Charged  

---

### 3️⃣ Stopping State

Occurs when you stop the instance.

**Actions performed:**
- OS shutdown begins  
- Compute resources are released  
- EBS volume is preserved  

👉 Temporary shutdown phase  

**Billing:** Compute charges stop  

---

### 4️⃣ Stopped State

**What happens:**
- Instance is powered off  
- Data remains stored on EBS  
- Instance can be restarted anytime  

👉 Useful for saving cost  

**Billing:**
- No compute charges  
- Storage charges apply  

---

### 5️⃣ Rebooting (Special Transition)

Reboot restarts the instance without stopping it.

- Same physical host  
- No data loss  
- Quick restart  

**Billing:** Continues  

---

### 6️⃣ Shutting-down State

Triggered when instance is terminated.

**Process:**
- AWS releases resources  
- Instance prepares for deletion  

---

### 7️⃣ Terminated State

Final lifecycle stage.

- Instance is permanently deleted  
- Cannot be restarted  

**Important:**
- Root volume may also be deleted (based on settings)  

**Billing:** Stops completely  

---

## 🔁 Lifecycle Flow Summary
