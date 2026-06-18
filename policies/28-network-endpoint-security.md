# 28 — Network & Endpoint Security Standard

| | |
|---|---|
| **Document ID** | POL-28 |
| **Policy Owner** | Chief Information Security Officer |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard / Regime** | ISO/IEC 27001:2022 (A.8.20–A.8.23, A.8.1, A.8.7); PCI-DSS Req. 1,5,11; MAS TRM |

---

## 1. Purpose

To define the technical controls protecting Aspire's networks and endpoints against unauthorised access, malware, and lateral movement, and to enforce segmentation that isolates sensitive environments such as the cardholder data environment.

## 2. Scope

All networks, network devices, cloud network constructs, and endpoints (servers, workstations, mobile) used to access or process Company data.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| Segmentation | Dividing networks to isolate sensitive zones. |
| EDR | Endpoint Detection and Response. |
| Zero Trust | Never-trust, always-verify access model. |
| WAF | Web Application Firewall. |
| Hardening | Reducing attack surface via secure configuration. |
| NAC | Network Access Control. |
| DDoS | Distributed Denial of Service. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| CISO | Owns network/endpoint security standards. |
| Network / Cloud Engineering | Implements segmentation, firewalls, and controls. |
| IT Endpoint Team | Manages endpoint baselines, EDR, and patching. |
| Security Operations | Monitors and responds to alerts. |

### 4.1 RACI

| Activity | CISO | Net/Cloud Eng | Endpoint | SecOps |
|---|---|---|---|---|
| Define network/endpoint baselines | A | R | R | C |
| Implement segmentation & firewalls | A | R | I | C |
| Deploy & manage EDR | A | C | R | C |
| Monitor & respond to alerts | A | C | C | R |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Network Security

Networks are segmented to isolate sensitive environments (e.g. the cardholder data environment per Policy 14). Default-deny firewall/security-group rules are enforced and reviewed regularly. Inbound web traffic is protected by a WAF and DDoS protection. Administrative interfaces are not exposed to the public internet. Remote access uses zero-trust/VPN with MFA (Policy 02).

## 6. Endpoint Security

All endpoints enforce a hardened baseline: full-disk encryption (AES-256), automatic screen lock, current OS/patch levels, EDR/anti-malware, host firewall, and MDM enrolment. Endpoints failing baseline checks are quarantined from sensitive resources. Removable-media use is restricted and controlled.

## 7. Secure Configuration & Hardening

Systems are built from hardened baselines aligned to recognised benchmarks (e.g. CIS); no vendor default credentials; unnecessary services disabled; configuration drift detected and remediated.

## 8. Malware Defence

Anti-malware/EDR is deployed on applicable systems, kept current, and monitored. Suspicious detections feed the incident process (Policy 08).

## 9. Security Testing

Internal and external vulnerability scans run at least quarterly (and after significant change); penetration tests run at least annually; findings are remediated per the Vulnerability & Patch Management Standard (Policy the relevant policy).

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Network controls & segmentation | ISO 27001 A.8.20–A.8.22; PCI-DSS Req. 1 |
| Protection against malware | ISO 27001 A.8.7; PCI-DSS Req. 5 |
| Secure configuration | ISO 27001 A.8.9; PCI-DSS Req. 2 |
| Security testing | ISO 27001 A.8.8; PCI-DSS Req. 11 |
| Endpoint protection | ISO 27001 A.8.1 |

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
| Endpoints compliant with baseline | ≥ 98% | Monthly | IT Endpoint |
| EDR coverage on in-scope hosts | 100% | Monthly | SecOps |
| External scans passing | 100% | Quarterly | Net Eng |
| Firewall rule reviews completed | 100% | Semi-annually | Net Eng |

## 13. Related Documents

- Information Security Policy (01)
- Access Control Policy (02)
- PCI-DSS Policy (14)
- Vulnerability & Patch Management Standard (Policy 30)
- Logging, Monitoring & SIEM Standard (Policy 29)
- Cryptography & Key Management (11)

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
