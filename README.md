# aws-ec2-apache-static-website
Hosting a static website on Amazon EC2 using Apache Web Server
# Project Overview
This project demonstrates how to deploy and host a static HTML website on an Amazon EC2 instance using the Apache HTTP Server.
# Technologies Used
AWS EC2
Amazon Linux 2023
Apache HTTP Server
Linux
SSH
HTML
Implementation Steps
Launched an Amazon EC2 instance.
Configured Security Group inbound rules.
Connected to EC2 using SSH and a PEM key.
Installed Apache using DNF.
Started and enabled the Apache service.
Created an HTML homepage.
Tested the webpage using curl.
Accessed the website through the EC2 public IPv4 address.
Commands Used
sudo dnf update -y
sudo dnf install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
sudo systemctl status httpd
curl http://localhost
Result
Successfully deployed and accessed a static website hosted on an Amazon EC2 Linux instance using Apache.
Learning Outcomes
Understanding EC2 instances
Linux server administration
SSH connectivity
Security Group configuration
Apache web server management
Basic website deployment
