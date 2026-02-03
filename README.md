 # AWS VPC + EC2 Architecture Project

## 📌 Project Overview
This project demonstrates how to create a custom VPC in AWS, configure public and private subnets, attach an Internet Gateway, and launch an EC2 instance inside a public subnet.

## 🧱 Services Used
- Amazon VPC
- Subnets (Public & Private)
- Route Table
- Internet Gateway (IGW)
- EC2
- Security Group

## 🗺️ Architecture
- Custom VPC (10.0.0.0/16)
- Public Subnet (10.0.1.0/24)
- Private Subnet (10.0.2.0/24)
- Internet Gateway attached to VPC
- Public route table with 0.0.0.0/0 → IGW
- EC2 instance launched in Public Subnet

## 🌐 How Internet Access Works
The EC2 instance gets internet access because:
- It is in a public subnet
- Subnet is associated with a route table that has IGW route
- EC2 has a public IP
- Security Group allows HTTP (80) and SSH (22)

## 🧪 Output
A simple website hosted on EC2 using Apache HTTP server.

## 🎤 Viva Ready Line
A subnet becomes public when it has a route to an Internet Gateway.

## 📂 Files Included
- Architecture Diagram
- Step-by-step project notes
- Viva questions and answers
****
