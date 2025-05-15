# 🧪 Hands-On Labs – Class 6: Detection and Response

This section contains summaries and artifacts from the hands-on labs completed in **Course 6** of the Google Cybersecurity Certificate. These labs develop practical skills in **network monitoring**, **incident response documentation**, and **packet analysis** using real-world tools and scenarios.

---

## 📁 Lab 1: Research Network Protocol Analyzers

**🎯 Objective:**  
Compare two widely used packet analysis tools—**Wireshark** and **tcpdump**—to understand their strengths, interfaces, and practical use in cybersecurity investigations.

**📝 Summary:**  
Students analyze how Wireshark provides a GUI-based deep inspection environment, while tcpdump offers a lightweight command-line interface for efficient and remote captures. This lab reinforces packet-level visibility and filtering logic using real `.pcap` data.

**🛠️ Skills Gained:**  
- Use of **Wireshark** for visual inspection of packet structures  
- Use of **tcpdump** for CLI-based packet capture and filtering  
- Understanding protocol layers and packet dissection  
- Documentation of tool comparisons for forensic use

🔗 **[View Lab Summary](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-06-Sound-The-Alarm/ResearchNetworkProtocolAnalyzers.md)**

---

## 📁 Lab 2: Document Incident with Incident Handler’s Journal

**🎯 Objective:**  
Simulate a security analyst’s role in documenting a ransomware incident using a structured incident handler's journal template aligned with NIST guidelines.

**📝 Summary:**  
In this lab, a fictional healthcare clinic is targeted by ransomware via a phishing attack. The student documents the timeline, cause, and impact using the 5 W's method and additional reflection—developing habits essential to real-world incident response.

**🛠️ Skills Gained:**  
- Documentation using **incident handler’s journal**  
- Analysis of attack origin, methods, and impact  
- Use of **NIST incident response phases** in context  
- Communication and reporting fundamentals

🔗 **[View Journal Entry](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-06-Sound-The-Alarm/DocumentIncidentWIncidentHandlersJournal.md)**

---

## 📁 Lab 3: Analyze File with VirusTotal and Pyramid of Pain

**🎯 Objective:**  
Investigate a suspicious file hash using **VirusTotal**, extract threat intelligence, and classify indicators of compromise using the **Pyramid of Pain** framework.

**📝 Summary:**  
In this scenario, a financial employee downloads a malicious spreadsheet. Using the file’s SHA256 hash, students analyze the VirusTotal report to determine whether the file is malicious, extract related IoCs, and categorize them based on how painful they are for attackers to lose.

**🛠️ Skills Gained:**  
- Use of **VirusTotal** to analyze files and hashes  
- Identification of **IoCs**: hash, domain, IP, tools, artifacts, TTPs  
- Application of the **Pyramid of Pain** threat model  
- Enrichment of alert data with global threat intelligence

🔗 **[View Lab Report](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-06-Sound-The-Alarm/AnalyzeFileWithVirusTotalAndPyramidOfPain.md)**

---

## 📁 Lab 4: Respond to Phishing Alert Using Playbook Procedures

**🎯 Objective:**  
Follow a structured phishing playbook to investigate and respond to a malicious email alert using real-world SOC protocols.

**📝 Summary:**  
In this lab, a phishing email with a malicious attachment triggers a Medium severity alert. The file’s hash was verified as malicious. You act as a Level 1 SOC analyst to evaluate the incident, complete the 5 W’s, and decide whether to escalate the alert using the organization’s phishing playbook.

**🛠️ Skills Gained:**  
- Use of **incident response playbooks**  
- Alert evaluation using sender, subject, and file hash analysis  
- Ticket escalation based on evidence of compromise  
- Writing structured alert resolution comments

🔗 **[View Alert Response](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-06-Sound-The-Alarm/RespondToPhishingAlertUsingPlaybook.md)**

---
