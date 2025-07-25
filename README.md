AWS Auto-Scaling Web Application 

Project Overview
This project demonstrates how to build a scalable, secure web application on AWS that automatically adjusts the number of EC2 instances based on traffic demand. I used Auto Scaling, Elastic Load Balancer (ELB), RDS and SSL to create a highly available and secure web infrastructure. The entire setup is configured to handle variable traffic efficiently, with cost-effective scaling.

What I Built:
•	Auto-Scaling EC2 Instances: Automatically add or remove servers based on CPU usage.
•	Elastic Load Balancer: Distributes incoming traffic across multiple EC2 instances.
•	Amazon RDS: A secure, fully managed relational database to store application data.
•	SSL Certificate: Secured the website using HTTPS for data protection and trust.
  
Key Technologies Used:
•	Amazon EC2: For deploying and managing web servers.
•	Elastic Load Balancer (ELB): For distributing traffic to EC2 instances.
•	Auto Scaling: To automatically scale the number of EC2 instances based on demand.
•	Amazon RDS (Aurora MySQL): For secure database management.
•	AWS Certificate Manager (ACM): To request and manage SSL certificates for HTTPS.
  
Key Features:
•	Automatic Scaling: The app scales based on CPU usage (70% threshold).
•	Secure Communication: SSL certificates were implemented to ensure encrypted communication between users and servers.
•	High Availability: Using AWS’s multi-availability zone deployment ensures high availability.

Screenshots of Load Balancer, EC2 Instance, Auto Scaling Group 


How I Did It:
•	EC2 Setup: Launched EC2 instances with a custom AMI and configured user data to install and run a simple web server.
•	Auto Scaling Group: Configured the Auto Scaling group with a launch template and connected it to an ELB.
•	Load Balancer: Created an Application Load Balancer to distribute traffic evenly across instances.
•	Database Setup: Set up Amazon Aurora for data storage and secured it with proper security groups.
•	SSL Implementation: Requested a free SSL certificate using AWS Certificate Manager and attached it to the Load Balancer to enable HTTPS.

Deployment Steps:
•	Launch EC2 instances.
•	Set up an Auto Scaling group.
•	Create an Elastic Load Balancer (ELB).
•	Configure SSL with ACM.
•	Test auto-scaling functionality with the Load Balancer.
