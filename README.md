# AWS EC2 Static Website Hosting using Apache

## Project Overview

This project demonstrates how to deploy and host a static HTML website on an Amazon EC2 instance using Apache HTTP Server.

The website is hosted on a personal AWS account using Amazon Linux 2023.

## Technologies Used

- AWS EC2
- Amazon Linux 2023
- Apache HTTP Server
- Linux
- SSH
- HTML

## Architecture

User Browser → EC2 Public IPv4 → Security Group → Apache HTTP Server → HTML Website

## Implementation Steps

1. Launched an Amazon EC2 instance.
2. Configured Security Group inbound rules for SSH (22) and HTTP (80).
3. Connected to EC2 using SSH and a PEM key.
4. Updated the Amazon Linux 2023 system.
5. Installed Apache using DNF.
6. Started and enabled the Apache service.
7. Created a static HTML homepage.
8. Tested the website using curl.
9. Accessed the website through the EC2 public IPv4 address.

## Commands Used

### Update system
```bash
sudo dnf update -y
```

### Install Apache
```bash
sudo dnf install httpd -y
```

### Start Apache
```bash
sudo systemctl start httpd
```

### Enable Apache at startup
```bash
sudo systemctl enable httpd
```

### Check Apache status
```bash
sudo systemctl status httpd
```

### Test website
```bash
curl --silent --include http://localhost
```

## Verification

- Apache service: Active and running
- Apache startup: Enabled
- HTTP response: `200 OK`
- Browser access: Successfully verified

## Skills Demonstrated

- EC2 instance deployment
- SSH connectivity
- Linux package management
- Apache web server management
- AWS Security Group configuration
- HTTP testing using curl

## Project Outcome

Successfully deployed a static HTML website on a personal AWS EC2 instance using Apache HTTP Server.
