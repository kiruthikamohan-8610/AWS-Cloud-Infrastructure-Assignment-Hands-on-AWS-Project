AWS — 1-Day Assignment
Duration: 1 Day     Level: Beginner

Objective: Create basic cloud infrastructure, deploy storage/web content, configure IAM/security, and document the work.

Task 1: Create S3 Storage
Create an S3 bucket:

student-cloud-&lt;yourname&gt;-2026

Requirements
• Upload cloud.jpg

• Upload student-guide.pdf

• Upload notes.txt

• Configure the bucket as private

Students must demonstrate:
• Bucket creation

• File upload

• Private access

• Object download

Screenshot required

S3 Bucket<br/> nnn cloud.jpg<br/> nnn student-guide.pdf<br/> nnn notes.txt

Task 2: IAM Policy + Role

Create a custom IAM policy that allows:

s3:ListBucket<br/>s3:GetObject

Only for their own S3 bucket.

Policy concept:

EC2<br/> fl<br/>IAM Role<br/> fl<br/>Custom IAM Policy<br/> fl<br/>S3 Bucket

Requirement: Do NOT use AWS access keys on EC2.

Attach the IAM role to an EC2 instance.

From EC2, demonstrate:

aws s3 ls s3://YOUR-BUCKET<br/><br/>aws s3 cp s3://YOUR-BUCKET/cloud.jpg .<br/><br/>aws s3 rm

s3://YOUR-BUCKET/cloud.jpg

Expected result:

AccessDenied

This demonstrates least privilege.

Task 3: EC2

Create an EC2 instance.

Requirements

• Amazon Linux

• Appropriate small instance for the lab

• SSH access

• IAM role attached

• Install AWS CLI if necessary

• Access the S3 bucket using the role

Students must submit:

• EC2 Instance

• Private/Public IP

• IAM Role

• S3 access result


Task 4: AWS Networking

Create a basic VPC:

VPC<br/>10.0.0.0/16<br/> |<br/> nnn Public Subnet<br/> n 10.0.1.0/24<br/> n<br/> nnn Private Subnet<br/> 10.0.2.0/24

Students should explain:

• VPC

• Subnet

• Internet Gateway

• Route Table

• Security Group

• Public IP

• Private IP

Bonus: Launch EC2 in the public subnet and verify SSH/HTTP access.



AWS Cloud Infrastructure Assignment
📌 Project Overview

This project demonstrates hands-on implementation of core AWS cloud infrastructure services. The assignment covers cloud storage, identity and access management, networking, and compute resources using the AWS Management Console.

☁️ AWS Services Used
Amazon S3
Amazon EC2
AWS IAM
Amazon VPC
Route Tables
Internet Gateway
Security Groups
🗄️ Task 1 – Amazon S3

Created an S3 bucket for storing and managing objects.

Bucket Configuration
Created an S3 bucket
Configured the bucket for private access
Uploaded cloud.jpg
Uploaded student-guide.pdf
Uploaded notes.txt
Verified object access and download
S3 Screenshots

🔐 Task 2 – IAM

Configured AWS Identity and Access Management to control access to AWS resources.

🌐 Task 3 – VPC Networking

Configured the required VPC networking components.

Components
VPC
Subnet
Route Table
Internet Gateway
Security Group

🖥️ Task 4 – EC2

Configured an EC2 instance as part of the AWS infrastructure assignment.

🏗️ Architecture
                 AWS Cloud
                     │
                     ▼
                  VPC
                     │
          ┌──────────┴──────────┐
          │                     │
       Subnet                Amazon S3
          │                     │
         EC2              Cloud Storage
          │
     Security Group
          │
     Route Table
          │
   Internet Gateway
🎯 Key Learning Outcomes
Understanding AWS cloud infrastructure
Working with S3 storage and object management
Understanding IAM and access control
Creating and configuring VPC networking
Working with route tables and Internet Gateway
Launching and configuring EC2 resources
Understanding basic AWS security concepts
🛠️ Technologies

AWS | S3 | EC2 | IAM | VPC | Networking | Cloud Computing

📸 Project Evidence

Screenshots demonstrating the configuration and successful completion of each task are included in the aws assignment directory.
