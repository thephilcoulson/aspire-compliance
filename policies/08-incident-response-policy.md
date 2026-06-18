# 08 — Incident Response & Breach Management Policy

| | |
|---|---|
| **Policy Owner** | [CISO / Head of Security] |
| **Approved By** | [Executive] |
| **Version** | 1.0 (template) |
| **Effective Date** | [DATE] |
| **Review Cadence** | Annual (+ post-incident) |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022 (A.5.24–A.5.28); SOC 2; PDPA/GDPR breach rules |

---

## 1. Purpose

To ensure security and data breach incidents are detected, reported, contained, and resolved promptly, with appropriate regulatory and customer notification.

## 2. Scope

All security incidents affecting Company systems, data, or services, including those at third parties.

## 3. Definitions

- **Event:** An observable occurrence.
- **Incident:** An event that compromises (or threatens) CIA of information.
- **Data Breach:** Unauthorised access, disclosure, loss, or alteration of personal/regulated data.

## 4. Severity Classification

| Severity | Description | Example |
|----------|-------------|---------|
| SEV1 (Critical) | Major impact; data breach, service outage | Confirmed exfiltration of customer PII |
| SEV2 (High) | Significant but contained | Malware on a server; limited exposure |
| SEV3 (Medium) | Limited impact | Single compromised low-priv account |
| SEV4 (Low) | Minimal impact | Isolated policy violation |

## 5. Response Lifecycle

1. **Detect & Report** — anyone aware of an incident must report it immediately via [channel]. 24/7 reporting available.
2. **Triage & Classify** — Security assesses severity and activates the response team.
3. **Contain** — isolate affected systems; preserve evidence.
4. **Eradicate** — remove the cause (malware, access, vulnerability).
5. **Recover** — restore services securely; validate integrity.
6. **Post-Incident Review** — root-cause analysis and corrective actions within [defined SLA].

## 6. Incident Response Team

| Role | Responsibility |
|------|----------------|
| Incident Commander | Owns coordination and decisions |
| Security Lead | Technical investigation & containment |
| Communications | Internal/external messaging |
| Legal/Compliance | Regulatory & legal obligations |
| DPO | Privacy breach assessment |
| Executive Sponsor | Escalation & approvals |

## 7. Regulatory & Customer Notification

- **PDPA:** Notify the PDPC and affected individuals where a breach is likely to result in significant harm, within statutory timeframes.
- **GDPR:** Notify the supervisory authority within 72 hours where required; notify data subjects for high-risk breaches.
- **Financial regulators:** Notify per applicable obligations (e.g. MAS incident reporting).
- **Card data:** Follow PCI-DSS and card-scheme breach procedures (link to Policy 14).
- All notification decisions are documented and legally reviewed.

## 8. Evidence & Forensics

- Preserve logs and evidence with chain of custody for potential investigation or legal proceedings.

## 9. Testing

- Incident response plans and runbooks are tested at least annually (tabletop or simulation).

## 10. Enforcement & Review

Reviewed at least annually and after every SEV1/SEV2 incident.
