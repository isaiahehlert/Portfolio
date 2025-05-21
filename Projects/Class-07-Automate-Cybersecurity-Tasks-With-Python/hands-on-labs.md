# 🧪 Hands-On Labs – Class 7: Automate Cybersecurity Tasks With Python

This section summarizes the hands-on labs completed in **Course 7** of the Google Cybersecurity Certificate. These labs focus on automating security operations using **Python**, including file parsing, list filtering, and writing update algorithms to manage access controls.

---

## 📁 Lab 1: Update a File Through a Python Algorithm

**🎯 Objective:**  
Develop a Python script that reads a text file containing an allow list of IP addresses, compares it to a remove list, and updates the file by removing matching IP addresses.

**📝 Summary:**  
In this lab, I acted as a security analyst managing access to a restricted subnetwork. I created a Python algorithm that automates the process of checking an `allow_list.txt` file for any IPs listed in a `remove_list`, and removes those entries. This ensures access is restricted only to current, authorized users. I used file handling methods like `.read()`, `.split()`, and `.write()` along with a `for` loop and conditionals to implement the algorithm. The final version updates the file directly with the revised list.

**🛠️ Skills Gained:**  
- File handling using Python's `with open()` and `.read()`, `.write()` methods  
- String to list conversion with `.split()`  
- Iteration and conditional logic using `for` loops and `if in`  
- File update automation using `.remove()` and `"\n".join()`  
- Portfolio-level scripting with real access control logic

🔗 **[View Python Algorithm](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-07-Automate-Cybersecurity-Tasks-With-Python/UpdateAFileThroughAPythonAlgorithm.docx)**
