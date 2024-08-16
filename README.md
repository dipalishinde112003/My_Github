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

### Explanation:
- **Graph LR**: Specifies a left-to-right (horizontal) layout.
- **A[Client Machine 1]** and **C[Client Machine 2]**: Represent the client machines.
- **B[(Git Server)]**: Represents the Git server.
- Arrows indicate the direction of code push/pull between clients and the server.
- The `style` attributes are used to give the nodes specific colors and strokes, which can be adjusted according to your preferences.

### Displaying Icons:
GitHub's Markdown parser with Mermaid doesn't natively support icons for nodes. However, you can represent the clients and server symbolically using text within the brackets:

- **A[PC: Client Machine 1]** for PC symbol.
- **B[(Server: Git Server)]** for server symbol.

If you need actual icons, you might need to use other tools like PlantUML or draw.io, and then embed the image in your `README.md`. 

### How to Use:
1. Copy the code snippet into your `README.md` file.
2. When viewed on GitHub, the architecture diagram will display with the specified layout and symbols.




