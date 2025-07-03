# NIDS_IDS-IPS
## Network Intrusion Detection System (NIDS)

## Project Overview

This repository contains the implementation of a **Network Intrusion Detection System (NIDS)** developed as part of a collaborative cybersecurity project.

The goal was to configure a functional NIDS using tools such as **Suricata** to monitor simulated network traffic, detect suspicious behavior, and respond to potential threats in real time.

---

## Objectives

- Monitor and analyze network traffic using open-source NIDS tools
- Detect and alert for various attack types, including:
  - DDoS (e.g., ICMP flood, SYN-Flood)
  - SQL injection
  - Port scanning
- Develop custom detection rules for specific threat patterns
- Analyze NetFlow/IPFIX traffic records
- (future adjustments) Integrate machine learning models to improve detection accuracy

---

## Tools and Technologies

- **Suricata** – high-performance network IDS/IPS
- **GNS3** – network simulation platform
- **IPFIX/NetFlow** – flow monitoring for traffic analysis
- **Python** – for parsing logs and optional ML integration
- **OpnSense** - Opensource firewall
- (Optional) **Scikit-learn** / **TensorFlow** – ML models

---

## Methodology

1. **Network Simulation:**  
   A virtual network environment was built in **GNS3**, containing internal hosts, servers, and attacker nodes to simulate various threat scenarios.

2. **NIDS Configuration:**  
   Each NIDS was installed on monitoring nodes with traffic mirroring enabled.

3. **Rule Development:**  
   Custom rules were written to detect:
   - Port scans using Nmap
   - SQL injection payloads
   - ICMP flood attacks
   - Unusual connection behavior

4. **Traffic Collection and Analysis:**  
   Traffic was captured and analyzed using NetFlow/IPFIX. Alerts and logs were collected for further analysis.

5. **(Optional) Machine Learning Integration:**  
   Extracted traffic features were used to test ML models for classifying malicious behavior.

---
**<a href="https://github.com/pnovato/NIDS_IDS-IPS/raw/main/Sistema-de-Deteccao-de-Intrusoes-na-Rede-NIDS.pdf" target="_blank">View the Final Presentation (PDF)</a>**

**<a href="https://github.com/pnovato/NIDS_IDS-IPS/raw/main/Relatório LPI(2).pdf" target="_blank">View the Final Report (PDF)</a>**
---

## Deliverables

-  Fully functional NIDS schema
-  Custom detection rules
-  Example attack scripts for testing 
-  Final technical report
-  Project presentation

---

## Results

The system successfully detected multiple attack patterns under test conditions and issued appropriate alerts. Performance was evaluated through simulated scenarios, showing effectiveness in real-time detection and log analysis.

---

## Authors

This project was developed in collaboration by a cybersecurity research team.  
For more details, please refer to the report and presentation in this repository.

---


