# 🧠 PASTA Threat Modeling – Sneaker App

This document outlines a full threat modeling assessment of the sneaker trading mobile app using the **PASTA (Process for Attack Simulation and Threat Analysis)** framework.

---

## 🔎 I. Define Business and Security Objectives

- The app must allow users to **sign up, log in, and manage accounts** easily.
- **Data privacy** is a top priority to build user trust and meet compliance expectations.
- The app must **handle payments securely**, offering multiple checkout options and minimizing legal and fraud risks.

---

## 🧰 II. Define the Technical Scope

**Technologies used:**
- API  
- PKI (AES + RSA)  
- SHA-256  
- SQL  

**Prioritized Technology:**  
I would prioritize evaluating the **SQL backend** first, as it stores critical data such as sneaker listings, seller information, and transaction records. Poorly implemented SQL queries can introduce injection vulnerabilities. SQL’s central role in querying and managing business logic makes it a high-risk entry point for attackers and a vital target for validation and sanitization.

---

## 🧩 III. Decompose Application (Data Flow)

Based on the provided data flow diagram:

- The **search function** allows users to browse sneaker listings.
- The **SQL database** pulls sneaker inventory, which may include metadata like price, seller, and availability.
- User input directly interacts with the SQL backend—highlighting the need for **input validation** to prevent SQL injection attacks.

---

## ⚠️ IV. Threat Analysis

- **External Threat:** SQL injection attacks targeting poorly sanitized inputs in search or payment forms.
- **Internal Threat:** Insider misuse—an employee or developer misusing access to payment records or user account data.

---

## 🛠️ V. Vulnerability Analysis

- The **SQL backend** could be vulnerable to injection attacks if inputs aren’t sanitized or if prepared statements aren’t used.
- **PKI flaws** or improper implementation could lead to man-in-t

---

## 🌲 VI. Attack Modeling

From the attack tree:

- **User data compromise** via SQL injection (e.g., lack of prepared statements).
- **Session hijacking** or brute-force attacks due to weak login mechanisms.
- **Payment manipulation** through insecure API endpoints.

---

## 🛡️ VII. Risk Analysis and Impact – Security Controls

1. **Input validation & parameterized SQL queries** to prevent injection.
2. **Multi-factor authentication (MFA)** to protect user accounts and prevent session hijacking.
3. **Use of secure HTTPS and TLS certificates** with PKI to ensure secure data exchange.
4. **Rate limiting and account lockout policies** to defend against brute-force attacks.

---

### 📌 Summary

This PASTA model highlights the major architectural and behavioral risks present in the sneaker trading app and provides actionable security controls aligned with best practices in modern mobile app development.
