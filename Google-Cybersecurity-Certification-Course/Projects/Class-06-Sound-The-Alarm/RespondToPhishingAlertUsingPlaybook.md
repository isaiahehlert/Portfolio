# 🛡️ Lab: Respond to Phishing Alert Using Playbook Procedures

This lab simulates the resolution of a phishing alert using a structured SOC playbook. You act as a Level 1 SOC analyst tasked with evaluating a suspicious file attachment and updating the alert ticket with findings.

---

## 📝 Alert Ticket Summary

**Ticket Status:** Escalated  
**Alert Type:** Suspicious email with malicious file attachment  
**Hash Investigated:** `54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b`

---

## 🔍 Ticket Comments

This phishing alert involved an employee receiving a password-protected spreadsheet attached to an email. The employee opened the file using a provided password, which triggered the execution of a malicious payload. The file's **SHA256 hash was verified as malicious** using VirusTotal, with over 50 vendors confirming it as a threat.

---

### ✅ Reasons for Escalation:

1. **Alert severity** is marked as **Medium**, which may require escalation per the Phishing Playbook.
2. The email **contained an attachment**, which was confirmed as **malicious** using VirusTotal.
3. The file triggered suspicious system behavior shortly after download, indicating potential compromise and requiring **Level 2 SOC analyst intervention**.

---

## 🧭 Playbook Path Followed

- **Step 2:** Evaluate the alert  
- **Step 3.0:** Email contains an attachment  
- **Step 3.1:** Attachment confirmed malicious  
- **Step 3.2:** Escalated with supporting details

---

## 🧠 Reflection

This exercise reinforces the importance of following structured procedures during incident response. Escalation paths minimize guesswork and ensure threats are addressed quickly by the appropriate personnel. Proper documentation, hash verification, and use of tools like VirusTotal are essential to protecting systems and data.
