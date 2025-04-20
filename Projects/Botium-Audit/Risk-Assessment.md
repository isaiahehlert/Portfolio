# 📊 Risk Assessment – Botium Toys (Updated)

This matrix identifies and evaluates key security risks found during the internal audit of Botium Toys, based on the official scenario report. Risk level is based on the likelihood of occurrence and the potential business or compliance impact.

| Risk Description                           | Likelihood | Impact   | Risk Level | Notes / Standards Affected         |
|-------------------------------------------|------------|----------|------------|------------------------------------|
| Missing encryption for sensitive data     | High       | High     | Critical   | GDPR, PCI DSS                      |
| No access control or least privilege policy| High       | High     | Critical   | Insider threat risk, noncompliance |
| Lack of intrusion detection/prevention    | High       | Medium   | High       | Weak detection = undetected attacks|
| Outdated/unsupported legacy systems       | Medium     | High     | High       | Patchless systems = malware risk   |
| No disaster recovery or backup strategy   | High       | High     | Critical   | Business continuity at risk        |
| Weak or reused employee passwords         | High       | Medium   | High       | Increased account compromise risk  |
| No centralized password manager           | Medium     | Medium   | Medium     | Password sprawl = poor hygiene     |
| Physical assets lack access logging       | Medium     | Medium   | Medium     | Can’t trace unauthorized access    |

**Overall Risk Score: 8/10**

> The organization has significant gaps in both administrative and technical controls. Priority should be placed on data protection, employee access management, system monitoring, and business continuity planning.
