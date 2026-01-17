# 🛠️ Mitigation Plan – Botium Toys (Updated)

This mitigation plan provides targeted actions to address the control gaps identified in the internal audit. Each recommendation aligns with the NIST Cybersecurity Framework and helps reduce Botium Toys’ risk posture.

---

| Issue Identified                        | Recommended Mitigation                                      | Control Category | Control Type     | Rationale / Benefit                                |
|----------------------------------------|--------------------------------------------------------------|------------------|------------------|---------------------------------------------------|
| Missing password policy                | Implement a strong password policy with complexity rules     | Administrative   | Preventative     | Reduces brute-force and credential reuse risks     |
| No password manager                    | Deploy a centralized password management system              | Technical        | Preventative     | Encourages unique, secure passwords across systems |
| No access control policy               | Define and enforce role-based access controls                | Administrative   | Preventative     | Enforces least privilege to reduce insider threats |
| No intrusion detection system          | Install IDS/IPS solution with alerting and logging           | Technical        | Detective        | Enables real-time monitoring and anomaly detection |
| Unencrypted sensitive data             | Implement AES-256 encryption for data at rest and TLS for transit | Technical    | Deterrent        | Meets compliance requirements and protects PII     |
| No backup or disaster recovery plan    | Schedule regular backups and document recovery procedures    | Technical        | Corrective       | Ensures continuity in case of breach or outage     |
| Incomplete employee training           | Standardize and require quarterly cybersecurity awareness training | Administrative | Preventative     | Strengthens human-layer defenses                  |
| Lack of inventory access logs          | Implement physical access logging for inventory systems      | Physical         | Detective        | Helps trace product movement and theft             |
