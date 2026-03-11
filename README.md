# 🛡️ Web Application Security & SOC Operations Lab

**Quick Summary:** An air-gapped, end-to-end cybersecurity home lab designed to simulate real-world web application attacks (Red Team) and implement centralized threat detection and monitoring (Blue Team). 

> ⚠️ **Disclaimer:** All artifacts and logs in this repository are sanitized. This lab is isolated. Do NOT run offensive tools against external/unauthorized systems.

---

## 🎯 Project Objective
To demonstrate practical competency in both offensive security (penetration testing) and defensive operations (SOC Tier 1/2 workflows) by building a complete attack-and-detect lifecycle.

## 💡 Capabilities & Skills Demonstrated
**🔴 Red Team (Offensive):**
* Executed web application vulnerability assessments targeting OWASP Top 10 flaws.
* Bypassed authentication mechanisms using proxy interception and credential stuffing.
* Automated database extraction via SQL Injection techniques.

**🔵 Blue Team (Defensive):**
* Engineered an isolated network architecture with strict firewall routing and NAT rules.
* Configured and tuned Network Intrusion Detection Systems (NIDS) to capture malicious traffic.
* Built centralized log ingestion pipelines (Syslog, Apache logs) into a SIEM.
* Developed custom SPL queries and dashboards for real-time threat hunting and incident correlation.

## 🛠️ Technology Stack
* **Attacker (Red):** Kali Linux, Burp Suite, SQLmap, Hydra, Netcat.
* **Defender (Blue):** Splunk Enterprise (SIEM), pfSense (Firewall), Snort (IDS/IPS).
* **Target Environment:** Ubuntu Server, Apache2, MySQL, DVWA (Damn Vulnerable Web App).
* **Infrastructure:** VirtualBox (Internal Networks/Air-gapped).

## 📚 Theoretical Foundations Applied
* **OWASP Top 10:** Deep understanding of SQL Injection (Error-based, Boolean) and Broken Authentication mechanisms.
* **Network Security & OSI Model:** Application of TCP/IP, ICMP vs. TCP routing, Outbound NAT, and packet filtering (L3/L4/L7).
* **Defense in Depth:** Implementing multi-layered security (Firewall segmentation → IDS monitoring → SIEM correlation).
* **SOC Operations:** Understanding the Incident Response lifecycle (Preparation, Detection & Analysis).

---
## 🚀 Quick Demo & Architecture
*(Chèn link ảnh/GIF Demo tấn công và Sơ đồ mạng của bạn vào đây)*
* **Network Topology:** [ARCHITECTURE.md](ARCHITECTURE.md)
* **Attack & Detect Flow:** `![Demo](recordings/demo-login-bruteforce.gif)`

---
*For detailed execution steps, rule configurations, and Splunk queries, please refer to the [docs/runbook.md](docs/runbook.md).*
