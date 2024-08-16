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

## Setting Up Cloud Server for Git

1. **Choose a Cloud Provider**: Select a cloud provider like AWS, Azure, or DigitalOcean.
2. **Create a Virtual Machine (VM)**: 
   - Example: For DigitalOcean, create a droplet with Ubuntu 20.04.
   
   ```bash
   ssh root@your-server-ip
