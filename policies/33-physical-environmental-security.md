# 33 — Physical & Environmental Security

| | |
|---|---|
| **Document ID** | POL-33 |
| **Policy Owner** | Head of IT / Facilities / CISO |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard / Regime** | ISO/IEC 27001:2022 (A.7); PCI-DSS Req. 9; SOC 2 |

---

## 1. Purpose

To protect Aspire's people, facilities, equipment, and information assets from physical and environmental threats — unauthorised access, theft, damage, and disruption — including controls over offices, data media, and (by reference) cloud data-centre providers.

## 2. Scope

All Aspire offices and facilities, physical assets and media, and the physical-security obligations of hosting/cloud providers.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| Secure Area | A controlled-access zone holding sensitive assets. |
| Access Badge | A credential for physical entry. |
| Visitor | A non-staff person on premises. |
| Clear Desk/Screen | Practice of securing information when unattended. |
| Media | Physical storage (disks, paper, backup tapes). |
| Environmental Controls | Protections against fire, power, climate threats. |
| Data Centre | A facility hosting IT infrastructure. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| Head of IT / Facilities | Owns physical security for offices and assets. |
| CISO | Sets physical-security requirements for information assets. |
| Facilities / Reception | Operate access control and visitor management. |
| All Staff | Follow clear-desk/screen and challenge unknown persons. |

### 4.1 RACI

| Activity | IT/Fac Head | CISO | Facilities | Staff |
|---|---|---|---|---|
| Maintain physical access controls | R | C | A | I |
| Manage visitors | I | I | A | R |
| Protect & dispose of media | C | A | R | R |
| Assure data-centre provider security | C | A | I | I |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Facility & Secure-Area Controls

Offices use access control (badges/biometrics) with least-privilege zoning; secure areas holding sensitive assets have stricter controls and access logging. Entry/exit is monitored; CCTV is used where lawful and proportionate. Access rights are reviewed regularly and revoked promptly on departure (Policy 06).

## 6. Visitor Management

Visitors are registered, identified, badged, and escorted in non-public areas; visitor logs are retained. Deliveries and contractors follow controlled-access procedures.

## 7. Clear Desk & Clear Screen

Staff secure Restricted/Confidential information when unattended, lock screens, and store sensitive documents/media securely. Printing of sensitive material uses secure print release where available.

## 8. Media & Equipment Protection

Physical media is inventoried, encrypted where applicable, transported securely, and disposed of by secure destruction (shredding/degaussing/crushing) with certificates retained (Policy 03, Policy 26). Equipment is protected from theft and environmental damage.

## 9. Environmental & Data-Centre Controls

Offices have appropriate fire detection/suppression, UPS/power protection, and climate control for equipment rooms. Production hosting relies on certified cloud/data-centre providers; their physical and environmental controls are validated via due diligence and assurance reports (Policy 07, Policy 27).

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Physical security perimeters & entry | ISO 27001 A.7.1–A.7.2; PCI-DSS Req. 9.1–9.2 |
| Protecting against physical/environmental threats | ISO 27001 A.7.5 |
| Clear desk & clear screen | ISO 27001 A.7.7 |
| Secure media handling & disposal | ISO 27001 A.7.10, A.7.14; PCI-DSS Req. 9.4 |
| Supporting utilities | ISO 27001 A.7.11–A.7.12 |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the the GRC exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the Head of IT and CISO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| Physical access reviews completed | 100% | Quarterly | Facilities |
| Visitor logs maintained | 100% | Monthly | Facilities |
| Secure-disposal certificates retained | 100% | Quarterly | Facilities |
| Clear-desk audit pass rate | ≥ 95% | Quarterly | CISO |

## 13. Related Documents

- Information Security Policy (01)
- Data Classification & Handling (03)
- HR Security Policy (06)
- Vendor & Third-Party Risk (07)
- Outsourcing & Cloud Governance (27)
- PCI-DSS Policy (14)

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
