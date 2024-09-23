# Virtual-Desktop-Infra
This package is a repository of scripts, configurations, and documentation on how to set up a VDI using Kasm Workspaces. Kasm Workspaces is a browser-based access to remote desktops and applications running in containers that offer a very scalable, secure, and customizable virtual environment.

# Key Features:

Containerized Desktops and Applications: Use containerized desktops and applications to enable smooth access from any browser.
Scalable architecture- This architecture is set and maintains virtual environments with an emphasis on scalability. 
It best addresses large user bases.
Security and Isolation: Use Kasm Workspaces native security features to create secure, isolated virtual sessions.
It can have customizable configurations related to the desktop environment, application access, and security policies of projects.
Automated Deployments: Shell scripts and templates for automatic installation and deployment of Kasm Workspaces across multiple platforms.
Documentation: Install, configure and scale VDI with Kasm using step-by-step guides.
# Technologies Used:
Kasm Workspaces
Docker
Kubernetes (optional, for large-scale deployments).
Linux (Ubuntu, CentOS, etc.) Nginx (for reverse proxy configuration) SSL/TLS for Safe Communication


# Steps to create VDI using Kasm Workspaces
1. Create an EC2 instance on any cloud platform for eg. AWS/Azure
2. Choose Ubuntu as AMI for your instance.
3. Choose key pair, either you can use old one or create a new.
4. Choose security group where you should allow ports like . (80,443,22).
5. After creating instance do ssh in the instance.
!(https://github.com/DevAg06/Virtual-Desktop-Infra/blob/main/Screenshot%20(367).png)

6. Then run following commands:
    - sudo apt update
    - cd /tmp
    - curl -O https://kasm-static-content.s3.amazonaws.com/kasm_release_1.16.0.f2d6e1.tar.gz
    - tar -xf kasm_release_1.16.0.f2d6e1.tar.gz
    - sudo bash kasm_release/install.sh
7. After running these commands you would be able to see some temporary passwords for users







 


