# Wazuh Manager Setup (Kali Linux)

## Steps

1. Update system:
   ```bash
   sudo apt update && sudo apt upgrade -y
2. **Install required Packages**
 sudo apt install curl apt-transport-https lsb-release gnupg -y
3. **Import Wazuh GPG and repo**
curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo apt-key add -
echo "deb https://packages.wazuh.com/4.x/apt/ stable main" | sudo tee /etc/apt/sources.list.d/wazuh.list
4. **Install Wazuh Manager**
sudo apt update
sudo apt install wazuh-manager -y
5. **Start services**
sudo systemctl enable wazuh-manager
sudo systemctl start wazuh-manager
6. **Check status**
sudo systemctl status wazuh-manager

✅ At this point, the Wazuh Manager should be running on Kali and listening for agent connections.
