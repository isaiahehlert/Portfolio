# 🧪 Hands-On Labs – Class 5: Detection and Response

This section contains summaries and artifacts from the hands-on labs completed in **Course 5** of the Google Cybersecurity Certificate. These labs focus on **monitoring, detection, and incident response**, using tools like **SIEMs (e.g., Splunk)** to investigate threats, filter event logs, and identify suspicious activity across assets and users.

---

## 🧰 Lab: Home Asset Inventory

**Course:**  
Google Cybersecurity Certificate – Class 05: Detection and Response

**Objective:**  
Identify and classify assets connected to a home office network to understand their importance and sensitivity, aiding in effective asset management and risk assessment.

**Scenario:**  
Operating a small business from a home office, I cataloged network-connected devices such as desktop computers, smart devices, and storage hardware. This asset inventory serves as a core reference for securing sensitive data and ensuring operational continuity.

**Tasks Completed:**
- Identified three previously undocumented network-connected assets.
- Documented ownership, location, and network access characteristics.
- Analyzed risk exposure and sensitivity of each asset.
- Classified devices using standardized sensitivity categories: *Confidential*, *Restricted*, *Internal-only*, and *Public*.

**Deliverable:**  
📄 [HomeAssetInventory.csv](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-05-Detection-and-Response/HomeAssetInventory.csv)

---

## 🛡️ Lab: Risk Register Assessment

**Course:**  
Google Cybersecurity Certificate – Class 05: Detection and Response

**Objective:**  
Evaluate potential threats to a financial institution and assign risk scores based on likelihood and severity. Use a risk register to prioritize mitigation strategies and ensure compliance with operational and regulatory requirements.

**Scenario:**  
A commercial bank in a coastal region with strict financial regulations and a hybrid workforce conducted a risk assessment of its funds. Key risks included business email compromise, database exposure, and supply chain issues. The team assessed risk exposure using NIST’s risk calculation formula: *Likelihood × Severity = Priority*.

**Tasks Completed:**
- Assessed five financial risks to banking operations.
- Assigned likelihood and severity scores using a 1–3 scale.
- Calculated priority scores to rank the risks.
- Documented the rationale behind each threat score in a register.

**Deliverable:**  
📄 [RiskRegister.csv](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-05-Detection-and-Response/RiskRegister.csv)

---

## 🔒 Lab: Data Leak Risk Assessment

**Course:**  
Google Cybersecurity Certificate – Class 05: Detection and Response

**Objective:**  
Evaluate the failure of least privilege controls following an internal data leak and recommend security control enhancements using NIST SP 800-53: AC-6 guidelines.

**Scenario:**  
A sales manager accidentally left internal-only documents shared with the team after a product meeting. A sales representative later sent the entire folder to an external partner who published the contents publicly. The breach was traced back to improper privilege revocation and poor access management.

**Tasks Completed:**
- Analyzed the breakdown of the least privilege principle.
- Reviewed NIST SP 800-53 AC-6 guidance on privilege enforcement.
- Recommended role-based access control and automatic privilege revocation.
- Justified solutions by highlighting prevention and damage control benefits.

**Deliverables:**  
📄 [DataLeakWorksheetTemplate.docx](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-05-Detection-and-Response/DataLeakWorksheetTemplate.docx)  
📄 [DataLeakWorksheet.csv](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-05-Detection-and-Response/DataLeakWorksheet.csv)

---

## 🧩 Lab: Access Control Assessment

**Course:**  
Google Cybersecurity Certificate – Class 05: Detection and Response

**Objective:**  
Investigate an access control failure involving improper authentication or authorization, and recommend remediation strategies based on the security principle of **least privilege**.

**Scenario:**  
A user accessed sensitive resources using an account that should have been deactivated. The incident triggered a post-incident access control review to determine the scope, origin, and appropriate mitigation steps. This lab exercise documents threat details, identifies the access control issue, and recommends controls to prevent recurrence.

**Tasks Completed:**
- Identified **who** caused the incident, **when** it occurred, and **what device** was used.
- Determined the user’s **level of access** and whether the account should have been active.
- Applied **authorization and authentication** concepts to classify the failure.
- Recommended **technical and managerial controls** such as:
  - Enforcing **automated account deprovisioning**.
  - Conducting regular **access reviews**.
  - Implementing **multi-factor authentication** and **logging triggers** for privileged access.

**Deliverable:**  
📄 [Sentinel_Access_Control_Assessment.docx](https://github.com/isaiahehlert/Portfolio/blob/main/Projects/Class-05-Detection-and-Response/Sentinel_Access_Control_Assessment.docx)
