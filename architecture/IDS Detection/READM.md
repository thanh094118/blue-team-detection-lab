## IDS Detection

Network traffic generated from the attack simulation was monitored using  
[Snort](https://www.snort.org/), an open-source Network Intrusion Detection System (IDS).

Snort inspects network packets and matches them against known attack signatures to identify suspicious activity.

### Detection Examples

**Web Attack Detection**

Snort generated alerts when malicious HTTP requests were detected, including:

- SQL Injection attempts in web parameters
- Suspicious HTTP query patterns
- Repeated login attempts indicating brute-force activity

Example alert:


[] [1:2010935:3] WEB-ATTACK SQL Injection attempt []
Classification: Web Application Attack
Priority: 1
Source IP: 192.168.x.x


### Security Monitoring

Detected events were forwarded to the monitoring stack and correlated with web server logs for investigation.


Attack Traffic → Snort IDS Alert → SIEM Log Correlation


This step demonstrates how IDS tools provide early detection of network-based attacks within a SOC monitoring environment.