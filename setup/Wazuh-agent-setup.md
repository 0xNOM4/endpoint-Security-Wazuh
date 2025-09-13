# Wazuh Agent Setup (Windows)

This document explains how I installed and configured the **Wazuh Agent** on a Windows machine and connected it to the Wazuh Manager running on Kali Linux.

---

## 🛠 Steps

### 1. Download the Wazuh Agent
- Go to the official download page:  
  [Wazuh Agent MSI](https://packages.wazuh.com/4.x/windows/wazuh-agent-4.x.msi)

### 2. Run the installer
- During setup:
  - **Wazuh Manager IP** → Enter the IP address of your Kali VM (for example: `192.168.1.55`)
  - Keep all other options as default.
- Complete the installation.
  ### screenshot: Agent Installation
  ![Agent setup]("C:\Users\the Comp Shop\Pictures\Screenshots\Screenshot 2025-09-12 111037.png")

### 3. Start the agent service
Open **Command Prompt (Admin)** and run:
```cmd
sc start wazuh
sc query wazuh
