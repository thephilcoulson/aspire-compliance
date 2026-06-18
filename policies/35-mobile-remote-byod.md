# 35 — Mobile, Remote Working & BYOD

| | |
|---|---|
| **Document ID** | POL-35 |
| **Policy Owner** | Chief Information Security Officer / Head of IT |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard / Regime** | ISO/IEC 27001:2022 (A.6.7, A.7.9, A.8.1); SOC 2 |

---

## 1. Purpose

To secure remote working and the use of mobile and personally-owned (BYOD) devices accessing Company data, balancing flexibility with protection of customer and corporate information.

## 2. Scope

All staff working remotely and all mobile/BYOD devices used to access Company systems or data.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| Remote Working | Working from outside Company premises. |
| BYOD | Bring Your Own Device — personal devices used for work. |
| MDM/MAM | Mobile Device / Application Management. |
| Containerisation | Isolating Company data within a managed app/profile. |
| Remote Wipe | Erasing Company data from a lost/stolen device. |
| Trusted Network | An approved, secured network for access. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| CISO / Head of IT | Own remote/BYOD security requirements. |
| IT Endpoint Team | Operate MDM/MAM and enforce baselines. |
| Managers | Approve remote/BYOD arrangements. |
| Staff | Comply with device and remote-working rules. |

### 4.1 RACI

| Activity | CISO/IT | Endpoint | Managers | Staff |
|---|---|---|---|---|
| Define remote/BYOD baselines | A | R | C | I |
| Enrol & manage devices (MDM/MAM) | A | R | I | C |
| Approve remote/BYOD access | C | I | A | R |
| Report lost/stolen devices | A | R | C | R |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Remote Working Controls

Remote access uses encrypted channels (VPN/zero-trust) with MFA (Policy 02). Staff work over trusted networks, avoid public Wi-Fi for sensitive work (or use VPN), maintain physical security of devices and screens, and apply clear-desk/screen practice (Policy 33). Sensitive calls/data are handled privately.

## 6. Device Baselines

All devices accessing Company data enforce: full-disk encryption (AES-256), screen lock with timeout, current OS/patches, endpoint protection, and MDM/MAM enrolment. Jailbroken/rooted devices are prohibited from accessing Company data.

## 7. BYOD Specifics

BYOD access uses containerisation/MAM to separate Company data from personal data, enabling selective remote wipe of Company data without affecting personal content. BYOD is permitted only with manager approval and acceptance of the BYOD terms; unsupported devices are denied access.

## 8. Lost / Stolen Devices

Lost or stolen devices are reported immediately to IT/Security (Policy 08); Company data is remotely wiped and access credentials rotated.

## 9. Offboarding

On departure or role change, Company data and access are removed from all devices, including BYOD (selective wipe), per the HR Security Policy (06).

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Remote working security | ISO 27001 A.6.7 |
| Security of assets off-premises | ISO 27001 A.7.9 |
| Endpoint/user device protection | ISO 27001 A.8.1; SOC 2 CC6.7 |
| Access control & MFA | ISO 27001 A.8.5; Policy 02 |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the the GRC exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CISO and Head of IT and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| Devices enrolled in MDM/MAM | ≥ 98% | Monthly | Endpoint |
| BYOD devices containerised | 100% | Monthly | Endpoint |
| Lost-device wipes completed within SLA | 100% | Per event | IT |
| Non-compliant devices blocked | 100% | Monthly | Endpoint |

## 13. Related Documents

- Acceptable Use Policy (05)
- Access Control Policy (02)
- Network & Endpoint Security Standard (28)
- HR Security Policy (06)
- Physical & Environmental Security (33)
- Incident Response (08)

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
