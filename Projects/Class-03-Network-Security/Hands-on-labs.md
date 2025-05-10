# Hands-On Labs – Class 3

This section will contain summaries and screenshots (if applicable) of the hands-on labs from this course, including:

- Network mapping
- Traceroute analysis
- Firewall configuration
- VPN usage
- Wireshark traffic capture

  ## 🧪 DNS & ICMP Network Traffic Analysis Lab

As part of the Google Cybersecurity Certificate coursework, this lab involved using `tcpdump` to analyze network traffic. The investigation focused on DNS and ICMP behavior when a DNS server fails to respond.

### 🔍 Files Submitted:
- 📝 [Final Completed Incident Report](./Final_Completed_Cybersecurity_Incident_Report_All_Steps.docx)
- 📄 [Blank Incident Report Template](./Cybersecurity-incident-report-network-traffic-analysis.docx)
*(Note: GitHub cannot preview .docx files. Click "Download" in the upper-right corner to view.)*

### 📌 Summary
The report captures a full analysis of a “destination port unreachable” issue linked to failed DNS queries over UDP. The ICMP response logs were used to isolate the root cause and propose remediation steps. This document demonstrates hands-on protocol analysis and incident response.

## 🧪 SYN Flood DoS Attack Investigation Lab

As part of Class 03: Network Security, this hands-on lab involved detecting and analyzing a SYN flood attack using packet captures and structured incident reporting. The lab simulated a real-world Denial of Service (DoS) event where a malicious actor disrupted web server availability by sending a high volume of TCP SYN packets without completing the handshake.

The objective was to identify the attack using packet sniffing tools (like Wireshark), document its impact using a formal incident report, and propose strategies to mitigate future risks. This lab applies key TCP/IP model concepts — including connection handshakes and protocol behavior — to analyze active threats in real network logs.

### 🔍 Files Submitted:
- 📝 [Completed Cybersecurity Incident Report](./CyberSecurityIncidentReport.docx)
- 📄 [Blank Incident Report Template](./CyberSecurityIncidentReportTemplate.docx)
*(Note: GitHub cannot preview .docx files. Click "Download" in the upper-right corner to view.)*

### 📌 Summary
This report documents a SYN flood DoS attack, where TCP connections were left half-open to exhaust server resources. Analysis of the Wireshark logs shows a high frequency of SYN packets from a single IP without follow-up ACKs. This hands-on investigation reinforces concepts like TCP handshakes, packet analysis, and mitigation tactics such as SYN cookies and rate limiting. It highlights the importance of proactive traffic inspection and firewall configuration in defending against denial of service threats.

## 🧪 Malware Redirect and Brute Force Breach Investigation Lab

This hands-on lab, part of Class 03: Network Security, involved analyzing an incident where a former employee compromised a company's web server via brute force and injected JavaScript into the website source code. The malicious code prompted visitors to download an executable file, which then redirected their browsers to a fake website hosting malware.

The lab involved using a sandbox environment and `tcpdump` to analyze DNS and HTTP traffic. Analysts traced the attack by reviewing DNS resolutions and HTTP GET requests in the packet log, confirming that visitors were redirected from `yummyrecipesforme.com` to `greatrecipesforme.com`. The root cause was traced to weak admin credentials and a lack of brute force protections.

### 🔍 Files Submitted:

- 📝 [Completed Security Incident Report](./Security_Incident_Report.docx)
- 📄 [Blank Incident Report Template](./Security-incident-report-template.docx)  
*(Note: GitHub cannot preview .docx files. Click "Download" in the upper-right corner to view.)*

### 📌 Summary

The report documents how a brute force attack was used to compromise a web server and distribute malware via browser redirection. Packet analysis showed HTTP and DNS traffic consistent with an injected redirect. The investigation reinforces critical topics like brute force mitigation, protocol behavior, and the risks of JavaScript-based attacks. A prevention strategy recommending two-factor authentication (2FA) was proposed to strengthen account security and reduce future risk.
