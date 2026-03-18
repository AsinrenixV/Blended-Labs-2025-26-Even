# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
---
**Author : ASIN RENIX V**
**Reg no : 212224040036**
**Date : 18-03-2026**
---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

```
1.Launched a new EC2 instance named Web Server in the N. Virginia region using Amazon Linux 2023 AMI and t2.micro instance type.
2.Enabled termination protection and stop protection, configured a security group, and added a user data script to install and start an Apache web server.
3.Monitored the instance using status checks, CloudWatch metrics, and system logs to ensure it was running properly.
4.Modified the security group to allow HTTP (port 80) traffic and accessed the web server using the public IP address.
5.Resized the instance to t2.small, increased the EBS volume size, explored EC2 service quotas, tested stop protection, and finally stopped the instance.
```

## Output Screenshots 

<img width="1919" height="888" alt="Screenshot 2026-03-18 212757" src="https://github.com/user-attachments/assets/4bf9dc94-8dee-4b92-8264-3f609d1736a5" />
<img width="1919" height="887" alt="Screenshot 2026-03-18 214900" src="https://github.com/user-attachments/assets/d6ef6df3-34b3-4720-8bc8-54b99da8a7a6" />
<img width="1918" height="893" alt="Screenshot 2026-03-18 220556" src="https://github.com/user-attachments/assets/423e1fac-7e29-4a05-9365-f2b1274cf4a6" />
<img width="1919" height="882" alt="Screenshot 2026-03-18 221512" src="https://github.com/user-attachments/assets/c4781875-9327-4775-81a6-383f13adf00f" />



## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
