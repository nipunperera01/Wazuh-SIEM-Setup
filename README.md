# 🛡️ Wazuh SIEM Setup – Ubuntu Server with Linux & Windows Agents

This project demonstrates a real-world Security Information and Event Management (SIEM) setup using [Wazuh](https://wazuh.com). It includes a central Ubuntu-based Wazuh server monitoring both Linux and Windows endpoints. The goal is to simulate a SOC (Security Operations Center) environment suitable for cybersecurity learning, monitoring, and analysis.

---

## 📌 Project Overview

- 🔧 **Wazuh All-in-One Server** on Ubuntu Server
- 🐧 **Ubuntu Client VM** acting as a Linux agent
- 🪟 **Windows Machine** added as a Windows agent
- 📡 Real-time log collection and event monitoring
- 📊 Visualization through Wazuh Dashboard (based on Kibana)

---

## 🖥️ Architecture Diagram

[ Windows Agent ] [ Ubuntu Agent ]
| |
+-------> [ Wazuh Server (Ubuntu) ]
|
[ Wazuh Dashboard (Web) ]


---

## 🚀 Tools & Technologies

- Wazuh 4.x (SIEM)
- Ubuntu Server 22.04 LTS
- Windows 11 Pro
- VMware Workstation / Oracle VirtualBox
- OpenSearch / Filebeat / Kibana-like Dashboard
- Linux CLI, systemd, SSH

---

## 🔐 Key Features

- 📡 Linux & Windows log collection
- ⚠️ Detection of SSH brute-force attempts
- 🔍 Monitoring failed logins, privilege escalations, suspicious activity
- 🧠 Hands-on SOC simulation for learning threat detection

---

## ⚙️ Setup Process

### 1. Wazuh All-in-One Server (Ubuntu)

- Installed using Wazuh-provided script
- Dashboard exposed on `https://<server-ip>:443`
- Wazuh manager, indexer, dashboard all on one VM

### 2. Linux Agent (Ubuntu)

- Installed Wazuh agent via APT repo
- Configured `/var/ossec/etc/ossec.conf` to connect to manager

### 3. Windows Agent

- Installed via `.msi` installer
- Connected to Wazuh server using agent-auth
- Monitored Event Viewer logs, USB events, and login activity

---

## 💼 Skills Demonstrated

-🧠 SIEM implementation and configuration
-🛠️ Linux and Windows log integration
-🔐 Cybersecurity monitoring and threat detection
-📦 OpenSearch and Filebeat pipeline understanding
-📁 Linux system configuration and automation

## Author

Nipun Perera
Undergraduate
NSBM Green University
