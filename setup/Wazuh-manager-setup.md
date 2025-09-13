# Wazuh Manager Setup (Kali Linux)

## Steps

1. Update system:
   ```bash
   sudo apt update && sudo apt upgrade -y
2. **Install required Packages**
   ```bash
    sudo apt install curl apt-transport-https lsb-release gnupg -y
4. **Import Wazuh GPG and repo**
   ```bash
    curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo apt-key add -
     echo "deb https://packages.wazuh.com/4.x/apt/ stable main" | sudo tee /etc/apt/sources.list.d/wazuh.list
5. **Install Wazuh Manager**
   ```bash
    sudo apt update
     sudo apt install wazuh-manager -y
6. **Start services**
   ```bash
     sudo systemctl enable wazuh-manager
      sudo systemctl start wazuh-manager
7. **Check status**
   ```bash
     sudo systemctl status wazuh-manager

✅ At this point, the Wazuh Manager should be running on Kali and listening for agent connections.

Screenshot:
![Manager Running](setup/wazuh_management_kali.png)

