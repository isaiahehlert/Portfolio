# 🧪 Lab: Analyze a Suspicious File with VirusTotal and the Pyramid of Pain

This lab involves investigating a potentially malicious file using VirusTotal and classifying its related indicators of compromise (IoCs) using the Pyramid of Pain framework.

---

## ✅ Has this file been identified as malicious?

**Yes**, the file has been identified as **malicious** by numerous antivirus vendors and corroborated by community analysis on VirusTotal.

- **SHA256 hash:** `54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b`
- Over **50 detection engines** flagged this file as malicious, using identifiers such as `Trojan.MalPack`, `Dropper.Generic`, and similar.
- The **Community Score** is **negative**, indicating high confidence of threat from experienced analysts.
- The **Behavior** tab shows:
  - Suspicious process creation  
  - Registry modification  
  - File system changes and outbound connections

---

## 🔺 Pyramid of Pain – Indicators of Compromise

### **TTPs (Tactics, Techniques, and Procedures)**
- `T1059.003` – **Command and Scripting Interpreter: Windows Command Shell**  
- `T1547.001` – **Boot or Logon Autostart Execution: Registry Run Keys**  
- `T1027` – **Obfuscated Files or Information**

### **Tools**
- Embedded use of **PowerShell scripts**
- Packed dropper used to deploy additional payloads
- Registry run key injection for persistence

### **Network/Host Artifacts**
- File created in `C:\Users\Public\` with randomized names  
- Attempts to schedule tasks for persistence  
- Modifies `HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run`

### **Domain Names**
- `update-checker.win` (flagged as malicious by several vendors)

### **IP Addresses**
- `185.193.127.179`  
  - Multiple detections  
  - Confirmed connection attempts during sandbox execution  

### **Hash Values**
- **SHA1:** `4d2c14777f7a6b9f9bc54e8c61e1a8f177208d1e`  
- **MD5:** `cfe3e8f735a0ef0533c1ec81a0f86ad0`

---

## 🧠 Reflections

This lab reinforces the importance of threat intelligence platforms like VirusTotal for rapid validation of suspicious files. The Pyramid of Pain serves as a strategic model to help SOC analysts evaluate and prioritize which IoCs are most impactful to attackers when detected or blocked.
