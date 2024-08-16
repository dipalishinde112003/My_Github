Build Your Own Git Server with Gitweb
Overview

This project demonstrates the process of creating a custom Git server with Gitweb for UI.
Table of Contents

    Understanding Architecture
    Setting Up Cloud Server for Git
    Configuring Git Server
    Adding Custom SSH Keys
    Pulling and Pushing Code
    Understanding How Git Stores Commits
    Setting Up Git UI with Gitweb
    Conclusion
```mermaid
graph TD
    A[Client Machine 1] --> |Push/Pull| B[Git Server]
    C[Client Machine 2] --> |Push/Pull| B[Git Server]
    B --> |Pull/Push| A
    B --> |Pull/Push| C


