# 🛡️ Final Incident Handler's Journal – Class 06: Detection and Response

This document contains four journal entries created during the Detection and Response course of the Google Cybersecurity Certificate. These entries demonstrate incident investigation techniques, the use of cybersecurity tools, and personal reflection on learning progress.

---

## 📅 Entry 1

**Date:** May 14, 2025  
**Entry:** 1  
**Description:**  
Investigated a ransomware attack against a U.S. healthcare clinic using the incident handler's journal format. This exercise focused on identifying the core details of a real-world breach and practicing the 5 W's method to document incident response.

**Tool(s) used:**  
- **None** directly used, though threat intelligence and response coordination were central themes.

**The 5 W’s:**  
- **Who:** An organized cybercriminal group targeting healthcare.  
- **What:** Systems were encrypted after a phishing-based ransomware payload was executed.  
- **When:** Tuesday, 9:00 a.m.  
- **Where:** The internal network of the clinic.  
- **Why:** Phishing email successfully bypassed defenses, exploiting human behavior.

**Reflections/Notes:**  
This case reinforced the importance of user training and phishing detection systems. Incidents like this show that even strong technical controls can be bypassed if social engineering succeeds. Writing out the 5 W's helped clarify the full timeline and motivations behind the attack. It was also clear that proper incident documentation is crucial not just for response, but for future training and prevention. I found it helpful to walk through the incident as if I were the SOC analyst on call — thinking not just technically, but operationally. In a real environment, having an IR plan ready and rehearsed would make the response smoother.

---

## 📅 Entry 2

**Date:** May 14, 2025  
**Entry:** 2  
**Description:**  
Used VirusTotal to analyze a SHA256 file hash from a phishing attachment that executed a malicious payload. The goal was to determine if the file was malicious and document related IoCs using the Pyramid of Pain.

**Tool(s) used:**  
- **VirusTotal**: Used to search for threat verdicts across multiple vendors and extract IoCs such as IPs, domains, and behavioral patterns.  
- **Pyramid of Pain**: Framework used to categorize the usefulness and pain-level of various IoCs for adversaries.

**The 5 W’s:**  
- **Who:** Unknown attackers distributing malware via email attachments.  
- **What:** A malicious `.xls` file was opened, leading to system compromise.  
- **When:** File was opened at 1:13 p.m.  
- **Where:** Email system and affected endpoint.  
- **Why:** Targeted phishing email evaded basic detection controls.

---

## 📅 Entry 3

**Date:** May 15, 2025  
**Entry:** 3  
**Description:**  
Followed a phishing playbook to evaluate an alert, determine maliciousness, and decide whether to escalate or close the incident. This simulated real-world SOC ticket handling procedures.

**Tool(s) used:**  
- **Phishing Incident Playbook**: Helped walk through the escalation decision process.  
- **Alert Ticket System**: Used to log findings, document analysis, and escalate confirmed phishing attacks.

**The 5 W’s:**  
- **Who:** Malicious actor impersonating a trusted sender.  
- **What:** Email contained a password-protected malicious attachment.  
- **When:** Alert triggered at 1:20 p.m.  
- **Where:** Company mail server and user workstation.  
- **Why:** Targeted phishing to bypass AV filters via encrypted attachment.

---

## 📅 Entry 4

**Date:** May 15, 2025  
**Entry:** 4  
**Description:**  
Created and tested custom Suricata IDS rules to detect suspicious HTTP GET requests using packet capture files. Analyzed output in `fast.log` and `eve.json`.

**Tool(s) used:**  
- **Suricata**: Used to define custom rule logic and scan `.pcap` files for matching network patterns.  
- **jq**: Utilized to parse and extract meaningful alerts from Suricata’s JSON logs.

---

## 🧠 Final Reflections

This journal helped me internalize how important structured documentation is in cybersecurity. Each entry trained me to think like a SOC analyst — focused on clear, factual reporting, repeatable analysis, and accountability. I learned the importance of tools like VirusTotal, Suricata, and Splunk not just for detection, but for investigation and context gathering. The 5 W’s structure gave me a repeatable method to break down any incident. Looking back, I’m more confident identifying what questions to ask, how to interpret logs, and how to decide when to escalate an alert. I also saw how essential writing and communication are in this field — not just detecting threats, but clearly explaining what happened and what should be done next. This journal will be a valuable part of my portfolio and growth as a cybersecurity professional.

