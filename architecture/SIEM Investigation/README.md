## SIEM Investigation

Security events generated during the attack simulation were centralized and analyzed using  
[Splunk](https://www.splunk.com/) SIEM.

Logs from the DVWA web server and alerts from the IDS were ingested into Splunk to support security monitoring and investigation.

### Log Sources

- **Apache Access Logs** – HTTP requests generated during the attack simulation.
- **Apache Error Logs** – Server-side errors and abnormal request behavior.
- **Snort IDS Alerts** – Signature-based detection of suspicious network activity.

### Investigation Activities

Typical analysis tasks performed in Splunk include:

- Searching for suspicious HTTP requests in Apache logs
- Identifying repeated login failures from the same source IP
- Correlating IDS alerts with web server logs
- Tracing attacker activity across multiple events

### Example Analysis Workflow


Detect suspicious HTTP request in Apache access log

Identify related Snort IDS alert

Trace attacker IP and activity timeline

Investigate attack pattern and impact


This investigation process demonstrates how SIEM tools help SOC analysts detect and analyze security incidents using centralized log data.