# Build Your Own Git Server with Gitweb

## Overview

This project demonstrates the process of creating a custom Git server with Gitweb for UI.

## Table of Contents

- [Understanding Architecture](#understanding-architecture)
- [Setting Up Cloud Server for Git](#setting-up-cloud-server-for-git)
- [Configuring Git Server](#configuring-git-server)
- [Adding Custom SSH Keys](#adding-custom-ssh-keys)
- [Pulling and Pushing Code](#pulling-and-pushing-code)
- [Understanding How Git Stores Commits](#understanding-how-git-stores-commits)
- [Setting Up Git UI with Gitweb](#setting-up-git-ui-with-gitweb)
- [Conclusion](#conclusion)
- [Architecture](#architecture)

## Understanding Architecture

Git is a distributed version control system that allows multiple developers to work on the same project without overwriting each other's work. The architecture involves a server where the main repository is stored, and clients (developers) who clone, pull, and push changes to and from the server.

```mermaid
graph LR
    A[PC: Client Machine 1] -- Push/Pull --> B[(Server: Git Server)]
    B -- Push/Pull --> A
    
    C[PC: Client Machine 2] -- Push/Pull --> B
    B -- Push/Pull --> C

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style C fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#bbf,stroke:#333,stroke-width:2px

## Setting Up Cloud Server for Git

1. **Create an EC2 Instance on AWS**:
   - Log in to your AWS Management Console.
   - Navigate to the EC2 Dashboard and click on "Launch Instance."
   - Name your instance `My_Git_Server` and choose an Amazon Machine Image (AMI) like Ubuntu 20.04.
   - Select an instance type (e.g., t2.micro for the free tier).
   - Configure the instance and launch it with a key pair for SSH access.

2. **Connect to the EC2 Instance using SSH**:
   - Once the instance is running, note the public IP address or DNS name.
   - Connect to the instance using SSH from your terminal:
   
   ```bash
   ssh -i /path/to/your-key.pem ubuntu@your-ec2-public-ip
![Screenshot from 2024-08-16 11-12-57](https://github.com/user-attachments/assets/9579d128-1a09-4f54-8d64-a6527dc39edb)

