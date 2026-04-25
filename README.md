# Chativa: Self-Hosted Chat & E2EE Encrypted Messaging for SMEs
![License](https://img.shields.io/badge/License-Lifetime-blue.svg) ![Security](https://img.shields.io/badge/Security-E2EE-success.svg) ![Deployment](https://img.shields.io/badge/Deployment-On--Premise-orange)

**Chativa** is a high-performance, self-hosted messaging suite designed to eliminate third-party dependencies and secure internal team workflows over local or remote infrastructures. Built specifically for **SMEs** who refuse to compromise on data privacy.
<p align="center">
  <img src="https://raw.githubusercontent.com/sassisouid/chativa/main/assets/chativa-logo.png" alt="Chativa Logo" width="200" />
</p>

# Technical Capabilities

- **Zero-Knowledge Encryption**: Built-in E2EE ensures your payloads are unreadable in transit.
- **True Air-Gapped Environments**: Deploy on bare-metal or local subnets. Fully functional without an active internet connection.
- **Uncapped Scalability**: Host an unlimited numbers of agents and clients without per-seat licensing.
- **Native A/V Broadcasting**: Handles P2P WebRTC audio/video connections and encrypted binary storage out of the box.
- **AI-Ready Nodes**: Inject your own conversational agents (e.g., Gemini) directly into the neural routing system.

---
**Get Started:**

[Explore the Community Engine (Free Edition)](https://github.com/sassisouid/chativa/releases)

# Deployment Guide: Chativa Architecture & Installation

### Introduction to the Infrastructure
The deployment of **Chativa** has been engineered to be as seamless as the interface itself. Whether you choose a local installation for absolute "offline" privacy or a cloud hosting setup for global collaboration, our **Neural Core** engine adapts to your needs.

---

## I. System Prerequisites (Neural Prerequisites)

Before initiating the uplink, ensure your environment meets the following specifications:

#### 1. Local Deployment (PC / Windows)
*   **Operating System**: Windows 10 or 11 (64-bit Architecture).
*   **Database Engine**: An active **MongoDB** instance (Local installation or MongoDB Atlas cluster).
*   **Network Environment**: Port **5000** must be available to allow the Node.js server to communicate with the interface.
*   **Connectivity**: Internet access required only for the initial license synchronization.

#### 2. Remote Deployment (VPS / Node.js Cloud Hosting)
To ensure 24/7 global accessibility, Chativa must be deployed on a robust server infrastructure.
*   **Runtime Environment**: **Node.js v16** or newer.
*   **Transfer & Storage**: **FTP/SFTP** access for deploying the source files.
*   **Database**: MongoDB (Recommended: Atlas for high availability).
*   **Security (MANDATORY)**: A valid **SSL (HTTPS)** certificate.
    > [!IMPORTANT]
    > Audio/Video calls and camera/mic access are blocked by browsers on unsecured connections (HTTP). Switching to HTTPS is a required step to activate the WebRTC link.
*   **Network Protocols**: **WebSockets** authorization and Port **5000** opening.

---

## II. Installation Steps (Neural Ignition Sequence)

Follow this step-by-step protocol to activate your communication hub.

### A. Local Deployment (Quick Start)
1.  **Extraction**: Unzip the Chativa archive onto your local drive.
2.  **Ignition**: Run the `Chativa.exe` file (or the startup script).
3.  **Assistant**: Follow the Smart Assistant instructions to link your local MongoDB.

### B. Remote Hosting Deployment (Detailed)
Server-side deployment requires precision to guarantee a stable connection.

#### 1. Transferring Media via FTP/SFTP
Use a client like **FileZilla** or **WinSCP** to transfer the entire Chativa package to your server directory (usually `/var/www/` or your Node.js hosting root). 
*   *Tip: Transfer the compressed archive (.zip) to save time and preserve file integrity.*

#### 2. Extraction & Permissions
Once the transfer is complete:
- **Extraction**: Use your hosting panel's file manager or the `unzip` command via SSH to extract the files.
- **Access Rights**: Ensure the server has write permissions for the `uploads/` and `client/config/` folders.

#### 3. Linking the Access Point (URL)
Point your domain name to your server's IP address. Then, access the following URL to launch the Configuration Assistant:
`https://your-domain.com/installer`

#### 4. Service Initialization (Persistence)
To ensure Chativa stays operational after your console session is closed, it is recommended to use a process manager like **PM2**:
`pm2 start server.js --name "chativa-core"`

---

## III. Database Link Configuration (Logic)
During the configuration step in the assistant:
1.  Enter your **MongoDB URI**.
2.  Create your **Core Administrator** profile (Name, Email, Passcode).
3.  **Activate Protocol**: The system will proceed with final synchronization and redirect you to the **Neural Dashboard**.

---

## IV. Maintenance Recommendations
*   **Identity Backup**: Upon your first login, export your **Private Neural Key** from the profile settings. This is the only way to restore access to your encrypted files (E2EE) if you change machines.
*   **Updates**: The Chativa system periodically checks for component integrity. Ensure you keep your instance updated for the latest security patches.

**Congratulations. Your Chativa infrastructure is now active and secure.**
