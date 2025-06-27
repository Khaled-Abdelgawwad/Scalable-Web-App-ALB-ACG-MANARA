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
### EC2
Launch instances for the web app. These virtual servers run your application code and can be automatically created or removed based on demand.

### Application Load Balancer (ALB)
Distributes traffic across multiple instances. Acts as a smart traffic director that only sends requests to healthy servers and can handle SSL certificates.

### Auto Scaling Group (ASG)
Ensures instances scale based on demand. Automatically adds servers when busy and removes them when quiet, keeping your app available 24/7.

### Amazon RDS (Optional)
Backend database (MySQL/PostgreSQL) with Multi-AZ. Managed database service that handles backups, updates, and failover automatically.

### IAM
Role-based access to instances. Security service that controls what each server can access without storing passwords on the servers.

### CloudWatch & SNS
Monitor performance and send alerts. CloudWatch watches your system metrics, and SNS sends you notifications when something needs attention.

## Benefits

- **High Availability**: Your app stays online even if servers fail
- **Cost Effective**: Only pay for servers you actually need
- **Automatic Scaling**: No manual intervention needed during traffic spikes  
- **Secure**: Built-in security features and isolated network
- **Managed Database**: No database maintenance headaches
