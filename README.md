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
graph LR
    subgraph Clients
        A[Client Machine 1]
        C[Client Machine 2]
    end
    B[(Git Server)]
    A --> |Push/Pull| B
    C --> |Push/Pull| B

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style C fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#bbf,stroke:#333,stroke-width:2px



