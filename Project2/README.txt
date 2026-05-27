# 🖥️ AWS EC2 Server Commander — DecodeLabs Project 2

## Overview
Provisioned a Linux virtual server on AWS EC2, secured it with SSH key authentication and firewall rules, installed Nginx web server via command line, and deployed a live custom webpage — without touching a GUI after launch.

## What I Built
- Launched an EC2 instance on Amazon Linux 2023 (t3.micro)
- Created SSH key pair and secured .pem file permissions
- Configured Security Group firewall rules (Port 22, 80, 443)
- Connected remotely via SSH terminal
- Installed and deployed Nginx web server via command line
- Hosted a custom "Welcome to DecodeLabs" webpage on a live public IP

## Live URL
http://13.127.38.83

## Tech Stack
- AWS EC2
- Amazon Linux 2023
- Nginx Web Server
- SSH Key Authentication
- AWS Security Groups
- GNU Nano (terminal editor)

## File Structure
```bash
aws-ec2-server-commander/
├── index.html              # Custom Welcome to DecodeLabs webpage
├── setup.sh                # Nginx installation and deployment script
├── README.md               # Project documentation
├── LICENSE                 # MIT License
└── screenshots/
    ├── ec2-running.png     # EC2 instance Running status
    ├── ssh-connected.png   # SSH terminal access granted
    ├── nginx-active.png    # Nginx service active (running)
    └── live-webpage.png    # Custom page live in browser
```

## Key Concepts Learned
- Infrastructure as a Service (IaaS) — Full OS control
- Shared Responsibility Model — AWS secures hardware, you secure the logic
- SSH Key Authentication — Public key on server, private key never shared
- Security Groups as ALLOW-ONLY firewalls
- Principle of Least Privilege — SSH restricted to My IP only
- Cattle vs Pets — Infrastructure is disposable and replaceable
- Systemctl — Linux service management

## Screenshots
![EC2 Running](screenshots/ec2-running.png)
![SSH Connected](screenshots/ssh-connected.png)
![Nginx Active](screenshots/nginx-active.png)
![Live Webpage](screenshots/live-webpage.png)