# Scalable Web Application with ALB and Auto Scaling
![Image](https://github.com/user-attachments/assets/c1d2bdad-b5f4-4e2b-987a-bde8b64b8ac7)

## Architecture: EC2-based

Deploy a simple web application on AWS using EC2 instances, ensuring high availability and scalability with Elastic Load Balancing (ALB) and Auto Scaling Groups (ASG). The project demonstrates best practices for compute scalability, security, and cost optimization.

This architecture automatically handles traffic spikes by adding more servers when needed and removes them when traffic is low, helping you save money while keeping your application running smoothly.

## Project Overview

This project creates a production-ready web application infrastructure on AWS that can handle thousands of users simultaneously. The system automatically adjusts to traffic changes, ensuring your application performs well during both quiet periods and traffic spikes.

The architecture follows AWS best practices for security, reliability, and cost optimization. All components work together to create a fault-tolerant system that can recover from failures automatically.

## How It Works

1. **Traffic comes in** through the Application Load Balancer
2. **Load Balancer distributes** requests across healthy EC2 instances
3. **Auto Scaling monitors** CPU usage and request counts
4. **New instances launch** automatically when traffic increases
5. **Instances terminate** automatically when traffic decreases
6. **Database stores** application data with automatic backups

## Key AWS Services Used
