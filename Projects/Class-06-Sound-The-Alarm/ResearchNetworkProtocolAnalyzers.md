# 🧪 Wireshark vs. tcpdump – Tool Comparison

This document compares two foundational packet analysis tools: **Wireshark** and **tcpdump**. Both are essential in the detection and response phase of cybersecurity.

---

## 📊 Comparison Overview

### 🖥️ Wireshark
- GUI-based packet analyzer with a color-coded interface
- Ideal for deep inspection of packet structure and protocol layers
- Allows real-time capture and rich offline `.pcap` analysis
- Advanced filtering using display filters (e.g., `http.request`)
- Visual timeline and flow graph tools for communication mapping

---

### 💻 tcpdump
- Command-line tool for capturing and inspecting packet data
- Lightweight and efficient for use over SSH or in headless environments
- Supports BPF (Berkeley Packet Filter) syntax for precise filtering (e.g., `tcp port 80`)
- Suitable for automation and scripting in incident response workflows
- Can write to `.pcap` files for analysis in Wireshark

---

## 🔁 Similarities
- Both support live capture and offline `.pcap` file analysis
- Both can filter traffic by IP, port, and protocol
- Both are open-source and widely used in network forensics
- Compatible with the same packet formats and protocols

---

## 📁 Use Case Tips
- Use **Wireshark** when deep inspection and visual clarity are needed  
- Use **tcpdump** when working remotely or needing command-line automation  

---

