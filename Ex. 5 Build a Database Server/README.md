# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: ASIN RENIX V
* **Register Number**: 212224040036
* **Date of Submission**: 18-03-2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)

```
1.Launched a new EC2 instance named Web Server in the N. Virginia region using Amazon Linux 2023 AMI and t2.micro instance type.
2.Enabled termination protection and stop protection, configured a security group, and added a user data script to install and start an Apache web server.
3.Monitored the instance using status checks, CloudWatch metrics, and system logs to ensure it was running properly.
4.Modified the security group to allow HTTP (port 80) traffic and accessed the web server using the public IP address.
5.Resized the instance to t2.small, increased the EBS volume size, explored EC2 service quotas, tested stop protection, and finally stopped the instance.
```

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

<img width="1918" height="889" alt="Screenshot 2026-03-18 110855" src="https://github.com/user-attachments/assets/a2f19994-3268-4138-a80c-e627dea5bfb5" />

---

### Screenshot 2: Database Service Running

<img width="1919" height="896" alt="Screenshot 2026-03-18 204907" src="https://github.com/user-attachments/assets/dd0970a0-0758-48da-b6ed-7a3932357733" />


---

### Screenshot 3: Sample Database and Table

<img width="1919" height="892" alt="Screenshot 2026-03-18 211117" src="https://github.com/user-attachments/assets/bec78149-43ff-4625-a5c7-abe71ef45a75" />



---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst
