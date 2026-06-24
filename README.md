## SecureBank Web Application Penetration Test 🔐💳

<img width="479" height="323" alt="image" src="https://github.com/user-attachments/assets/305e16e0-fef8-46c6-b9f3-367868b28b90" />


A hands-on penetration testing project carried out against the SecureBank FinTech web application written in .NET and C# running in a controlled lab environment. The goal is to identify security weaknesses, understand their impact, and document practical remediation steps based on real-world attack scenarios.

---

##  Project Overview

SecureBank is an intentionally vulnerable banking application designed for security training. This project simulates a real penetration test to explore how attackers could exploit common web application flaws and how defenders can fix them 🛡️.

---

## ⚙️ Lab Setup

* 🎯 Target: SecureBank (Docker-based application)
* 💻 Attacker Machine: Kali Linux
* 🐳 Deployment: Docker / Docker Compose
* 🌍 Access: `http://localhost` or `http://<target-ip>`
* 🔑 Default Credentials:

  * [admin@ssrd.io](mailto:admin@ssrd.io) / admin
  * [developer@ssrd.io](mailto:developer@ssrd.io) / test

---

## 📁 Repository Structure 🗂️

```
SecureBank-Pentest/
│
├── 01-Reconnaissance/ 
├── 02-Authentication-Testing/ 
├── 03-Enumeration/ 
├── 04-Vulnerability-Analysis/ 
├── 05-Exploitation/ 
├── 06-Post-Exploitation/ 
├── 07-Reporting/ 
│
├── screenshots/ 
├── notes/ 
└── README.md
```

##   Methodology

### 1. 🔍 Reconnaissance & Enumeration

* Directory discovery using tools like Gobuster
* Technology fingerprinting
* Service and endpoint mapping

### 2. 🔐 Authentication Testing

* Weak/default credentials testing
* Login behavior analysis
* Session handling inspection

### 3. 🧩 Vulnerability Analysis

* OWASP Top 10 mapping 🧾
* Input validation testing
* Access control checks

### 4. 💥 Exploitation (Lab-safe validation)

* Controlled exploitation of discovered flaws
* Proof-of-concept testing in isolated environment

### 5. 📊 Post-Exploitation Analysis

* Impact assessment
* Data exposure evaluation
* Privilege escalation paths (if applicable)

### 6. 📝 Reporting

* Risk rating (Low / Medium / High / Critical)
* Technical findings
* Fix recommendations

---

##  Tools Used

*  Burp Suite
*  Docker / Docker Compose
*  Nmap
*  Gobuster
* Browser DevTools

---

## 📊 Key Findings 

*  Weak default credentials (admin/admin)
*  Hidden directories and endpoints discovered
*  Restricted admin panel access (403 responses)
*  Exposed API surface on port 5000
*  Misconfigured access controls and permissions

---

## ⚠️ Security Impact 

These issues could lead to:

* Unauthorized admin access
* Sensitive data exposure 
* Increased attack surface 
* Potential full application compromise in real environments

---

## 🛡️ Recommendations

*  Enforce strong password policies
*  Remove default credentials immediately
*  Restrict access to sensitive endpoints
*  Implement proper RBAC (Role-Based Access Control)
*  Secure APIs with authentication tokens
*  Disable unnecessary services and directory exposure
  
---

##  What is the purpose of me doing this;

This project is part of my cybersecurity learning journey focused on:

* Offensive security fundamentals 
* WebApp penetration testing 
* OWASP Top 10 practical exposure 
* Real-world security reporting skills 
* And in general just to secure Applications
---

