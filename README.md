# endpoint-Security-Wazuh
Implementing Endpoint Security &amp; Monitoring using Wazuh (EDR, File Integrity Monitoring, Automated Alerts).
##🎯Objective
Protect devices and servers from malware and unauthorized access.
📌 Deliverables
- ✅ Deploy EDR (Wazuh)
- ✅ Monitor file integrity and user activity
- ✅ Automate alerts for suspicious behavior

  ⚙️ Setup
- **Wazuh Manager** → Kali Linux VM
- **Wazuh Agent** → Windows Host
- Network configured with **Bridged Adapter**

   # 📂 Repository Structure
- `setup/` → Installation and configuration steps
- `configs/` → Custom Wazuh configuration files
- `screenshots/` → Screenshots showing running manager/agents
- `logs/` → Example alert logs

  # 🚀 How to Reproduce
1. Install Wazuh Manager on Kali  
2. Install Wazuh Agent on Windows  
3. Connect agent → manager  
4. Generate a file change → verify alert in Wazuh logs
