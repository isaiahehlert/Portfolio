# 🛡️ Mitigation Plan – Botium Toys Internal Audit

This plan outlines recommended actions to address the risks and gaps identified during the internal audit. It includes control types, categories, and the rationale for each recommendation.

---

| Issue Identified                  | Recommended Mitigation                                  | Control Category | Control Type     | Rationale / Benefit                                       |
|----------------------------------|----------------------------------------------------------|------------------|------------------|-----------------------------------------------------------|
| Missing separation of duties     | Assign critical roles to different personnel             | Administrative   | Preventative     | Reduces insider threat and single point of failure        |
| Outdated firewall firmware       | Update firmware and configure firewall rules             | Technical        | Preventative     | Reduces exposure to known vulnerabilities                 |
| No IDS/IPS system                | Deploy IDS/IPS to monitor and alert on traffic anomalies | Technical        | Detective        | Improves detection of real-time threats                   |
| Unencrypted PII storage          | Implement data encryption at rest and in transit         | Technical        | Deterrent        | Ensures confidentiality, meets GDPR/PCI DSS              |
| Missing server room locks        | Install physical locks and restrict access               | Physical         | Preventative     | Prevents unauthorized physical access to infrastructure   |
| No badge access logging          | Implement badge readers with logging and alerts          | Physical         | Detective        | Enables access tracking for accountability                |
| Employee phishing awareness low  | Provide mandatory quarterly security awareness training  | Administrative   | Preventative     | Strengthens human layer of defense                        |
