# 🎓 AWS 3-Tier Student Application Deployment

> A secure 3-Tier Student Registration Application deployed on AWS using EC2, VPC, RDS, Nginx, and Apache Tomcat.

---

# 📌 Project Overview

This project demonstrates the deployment of a highly available 3-tier web application on AWS. The application allows users to register student information through a web interface hosted on Apache Tomcat, with Nginx acting as a reverse proxy and Amazon RDS MySQL as the backend database.

---

# 🏗️ Architecture

```
                Internet
                    │
                    ▼
          Internet Gateway (IGW)
                    │
                    ▼
        Public Subnet (Nginx Server)
                    │
             Nginx Reverse Proxy
                    │
                    ▼
      Private Subnet (Tomcat Server)
                    │
        Student Registration App
                    │
                    ▼
      Private Subnet (Amazon RDS MySQL)

```

---

# 🛠️ AWS Services Used

- Amazon EC2
- Amazon VPC
- Public & Private Subnets
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- Amazon RDS (MySQL)
- Apache Tomcat
- Nginx

---

# 🚀 Features

- Secure 3-Tier Architecture
- Student Registration Application
- Reverse Proxy using Nginx
- Apache Tomcat Application Server
- Amazon RDS MySQL Database
- Public & Private Subnet Communication
- NAT Gateway for Internet Access
- Secure Network using Security Groups

---

# ☁️ Infrastructure

### VPC

| Resource | Value |
|----------|-------|
| VPC Name | VPC-3-tier |
| CIDR | 192.168.0.0/16 |

### Subnets

| Subnet | CIDR |
|---------|------|
| Public-Subnet-Nginx | 192.168.1.0/24 |
| Private-Subnet-Tomcat | 192.168.2.0/24 |
| Private-Subnet-Database | 192.168.3.0/24 |
| Public-Subnet-LB | 192.168.4.0/24 |

---

# 💻 EC2 Instances

| Instance | Purpose |
|----------|---------|
| Nginx Server | Reverse Proxy |
| Tomcat Server | Student Application |
| Amazon RDS | MySQL Database |

---

# 🗄️ Database

- Amazon RDS MySQL
- Database Name: **studentapp**
- Students table
- Secure private connectivity

---

# 🔧 Application Stack

- Apache Tomcat 9
- Java 11
- Nginx
- MySQL Connector
- Student WAR Application

---

# 🌐 Network Flow

```
Browser
    │
    ▼
Nginx (Public EC2)
    │
    ▼
Tomcat (Private EC2)
    │
    ▼
Amazon RDS MySQL
```

---

# 🎯 Learning Outcomes

- Designed a secure AWS 3-Tier Architecture.
- Configured Public and Private Subnets.
- Implemented Internet Gateway and NAT Gateway.
- Configured Route Tables and Security Groups.
- Deployed Apache Tomcat application on EC2.
- Configured Nginx Reverse Proxy.
- Connected Tomcat with Amazon RDS MySQL.
- Validated secure communication between Web, Application, and Database tiers.

---

# 👨‍💻 Author

**Ajit Swami**

AWS Cloud | DevOps | Python
