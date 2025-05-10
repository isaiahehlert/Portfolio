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

## 🧪 Network Hardening and Risk Assessment Lab

This lab focused on evaluating real-world network vulnerabilities within a simulated organization that had experienced a major data breach. As a security analyst, you were tasked with identifying unaddressed risks and recommending specific hardening practices to strengthen the company’s network infrastructure.

Four vulnerabilities were identified: shared passwords, default admin credentials, missing firewall rules, and lack of multifactor authentication (MFA). The risk assessment report outlines how to mitigate these issues using firewall rule enforcement, password policy enforcement, and MFA implementation.

### 🔍 Files Submitted:

- 📝 [Completed Security Risk Assessment Report](./Security_Risk_Assessment_Report.docx)
- 📄 [Blank Risk Assessment Template](./SecurityRiskAssessmentTemplate.docx)  
*(Note: GitHub cannot preview .docx files. Click "Download" in the upper-right corner to view.)*

### 📌 Summary

This report details a formal security assessment following a simulated data breach. It includes the selection of specific network hardening tools — such as firewalls and MFA — and explains how and when these methods should be implemented to reduce attack surfaces. The exercise reinforces essential practices in policy enforcement, access control, and network monitoring that are critical to maintaining a secure infrastructure.

## 🧪 NIST CSF-Based Incident Report – DDoS Attack Mitigation

In this final lab, you applied the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF) to analyze a real-world distributed denial of service (DDoS) attack. The attack targeted a multimedia company’s internal network via a flood of ICMP packets, exploiting an unconfigured firewall. This resulted in two hours of downtime and a full network lockdown.

The investigation involved breaking down the response using the five NIST CSF core functions: Identify, Protect, Detect, Respond, and Recover. As a security analyst, your role was to summarize the incident and propose long-term security strategies to prevent recurrence.

### 🔍 Files Submitted:

- 📝 [Completed Incident Report Analysis](./Incident_Report_Analysis.docx)
- 📄 [Incident Report Template](./IncidentReportAnalysisTemplate.docx)  
*(Note: GitHub cannot preview .docx files. Click "Download" in the upper-right corner to view.)*

### 📌 Summary

This lab demonstrates a methodical approach to post-incident analysis using the NIST CSF. The report outlines how unfiltered ICMP traffic enabled the attack and how future risk can be minimized through firewall tuning, source IP verification, and network segmentation. It also includes a recovery plan for staged service restoration and improved incident communication protocols.
