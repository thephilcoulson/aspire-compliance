# 29 — Logging, Monitoring & SIEM Standard

| | |
|---|---|
| **Document ID** | POL-29 |
| **Policy Owner** | Chief Information Security Officer |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard / Regime** | ISO/IEC 27001:2022 (A.8.15–A.8.16); PCI-DSS Req. 10; SOC 2 CC7.x; MAS TRM |

---

## 1. Purpose

To ensure security-relevant events are logged, protected from tampering, centrally monitored, and retained, enabling detection of and response to threats and supporting investigations and audits.

## 2. Scope

All production systems, applications, network devices, cloud services, and security tools generating security-relevant logs.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| Log | A time-stamped record of an event. |
| SIEM | Security Information and Event Management platform. |
| Correlation | Linking events to detect threats. |
| Use Case / Detection | A configured rule that generates a security alert. |
| Time Synchronisation | Consistent clocks across systems (NTP). |
| Tamper-proofing | Protecting logs from alteration/deletion. |
| SOC | Security Operations Centre. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| CISO | Owns logging/monitoring strategy and SIEM. |
| Security Operations | Operates the SIEM, triages and investigates alerts. |
| Engineering / IT | Ensures systems emit required logs. |
| Internal Audit | Reviews log coverage and integrity. |

### 4.1 RACI

| Activity | CISO | SecOps | Eng/IT | Internal Audit |
|---|---|---|---|---|
| Define logging requirements | A | R | C | I |
| Forward logs to SIEM | A | C | R | I |
| Build & tune detections | A | R | C | I |
| Monitor, triage & escalate alerts | A | R | I | I |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Logging Requirements

Systems log security-relevant events: authentication (success/failure), authorisation and privilege changes, access to Restricted data and cardholder data, administrative actions, configuration changes, and security-tool events. Logs capture who, what, when, where, and outcome. Clocks are synchronised via NTP to a trusted source.

## 6. Centralisation & Retention

Logs are forwarded to a central SIEM in near-real-time. Security logs are retained for **at least 12 months**, with **at least 3 months immediately available** for analysis (PCI-DSS Req. 10), and longer where law requires (Policy the relevant policy).

## 7. Integrity & Access

Logs are protected against unauthorised access, alteration, and deletion (write-once/immutable storage where feasible); access to logs is least-privilege and itself logged.

## 8. Monitoring, Detection & Triage

Detection use-cases cover priority threats (credential abuse, privilege escalation, data exfiltration, malware, anomalous payments). Alerts are triaged within SLA and escalated to the incident process (Policy 08); detections are tuned to manage false positives.

## 9. Review & Coverage Assurance

Log source coverage is reviewed regularly to ensure in-scope systems are logging; gaps are remediated. Daily review of critical alerts is performed by Security Operations.

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Event logging | ISO 27001 A.8.15; PCI-DSS Req. 10.2 |
| Monitoring activities | ISO 27001 A.8.16; SOC 2 CC7.2 |
| Clock synchronisation | ISO 27001 A.8.17; PCI-DSS Req. 10.6 |
| Log retention & protection | PCI-DSS Req. 10.5; ISO 27001 A.8.15 |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the the GRC exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CISO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| In-scope systems forwarding logs | 100% | Monthly | SecOps |
| Critical alerts triaged within SLA | ≥ 95% | Weekly | SecOps |
| Log retention meeting policy | 100% | Quarterly | CISO |
| Detection coverage of priority threats | ≥ 95% | Quarterly | SecOps |

## 13. Related Documents

- Information Security Policy (01)
- Incident Response (08)
- Network & Endpoint Security Standard (28)
- PCI-DSS Policy (14)
- Records Management & Retention (26)
- Detection Use-Case Catalogue

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
