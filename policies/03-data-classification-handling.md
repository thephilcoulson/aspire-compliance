# 3 — Data Classification & Handling Policy

| | |
|---|---|
| **Document ID** | POL-03 |
| **Policy Owner** | CISO / DPO |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022 (A.5.12–A.5.13, A.8.10–A.8.12); SOC 2 Confidentiality |

---

## 1. Purpose

To ensure information is classified according to its sensitivity and value, and handled with controls appropriate to its classification throughout its lifecycle — from creation through storage, transmission, sharing, and secure disposal. Correct classification underpins access control, encryption, retention, and privacy obligations across Aspire's platform.

## 2. Scope

All information assets, in any form (electronic, physical, verbal), created, received, owned, or processed by Aspire, and all personnel and systems that handle them.

## 3. Definitions & Glossary

| Term | Definition |
|------|------------|
| **Classification** | The assignment of a sensitivity level to information. |
| **Data Owner** | The accountable individual for a dataset's classification and use. |
| **Data Custodian** | The party operating the systems that store/process the data. |
| **PII** | Personally Identifiable Information. |
| **CHD / SAD** | Cardholder Data / Sensitive Authentication Data (see Policy 14). |
| **DLP** | Data Loss Prevention — controls detecting/blocking unauthorised data movement. |
| **Labelling** | Marking an asset with its classification. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| CISO | Owns the classification scheme and handling standard. |
| DPO | Ensures personal-data classification aligns with privacy obligations (Policy 04). |
| Data Owners | Assign and maintain classification; approve access and sharing. |
| Data Custodians / IT | Implement technical handling controls (encryption, DLP, access). |
| All Staff | Handle data per its classification and label new assets. |

### 4.1 RACI — Classification & Handling

| Activity | CISO | DPO | Data Owner | Staff |
|---|---|---|---|---|
| Define classification scheme | A | R | C | I |
| Classify assets | I | C | A | R |
| Apply handling controls | C | R | A | R |
| Approve external sharing of Restricted data | A | C | R | I |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Classification Levels

| Level | Definition | Examples |
|---|---|---|
| **Restricted** | Highest sensitivity; severe harm if disclosed. | Cardholder data (PAN), credentials, encryption keys, KYC/biometric data, full bank details, STR content. |
| **Confidential** | Sensitive business or personal data. | Customer PII, transaction records, contracts, source code, financials. |
| **Internal** | Internal-use information. | Internal docs, policies, project plans, non-public roadmaps. |
| **Public** | Approved for public release. | Marketing materials, published terms, public API docs. |

## 6. Handling Requirements (Procedures)

| Control | Restricted | Confidential | Internal | Public |
|---|---|---|---|---|
| Encryption at rest | Required | Required | Recommended | Optional |
| Encryption in transit | Required | Required | Required | Optional |
| Access control | Strict need-to-know + MFA | Need-to-know | Authenticated staff | Open |
| External sharing | Prohibited without DPO/CISO approval | Approval + agreement (DPA/NDA) | Limited | Permitted |
| DLP monitoring | Enforced | Enforced | Monitored | N/A |
| Retention | Per legal/regulatory schedule | Per schedule | Per schedule | N/A |
| Disposal | Secure wipe / cryptographic erase / shred | Secure wipe / shred | Standard delete | N/A |

## 7. Labelling

- Restricted and Confidential assets are labelled where technically feasible (document headers, metadata tags, repository tags).
- The default classification for unlabelled internal data is **Internal**.
- Aggregations that increase sensitivity are classified at the higher level.

## 8. Storage, Transmission & Endpoints

- Restricted and Confidential data must reside only in approved systems and locations (no shadow IT, no personal cloud storage).
- Transmission outside Aspire requires encryption and, for personal data, a lawful basis and appropriate safeguards (Policy 04).
- Endpoint controls (encryption, DLP, MDM) protect data on devices per the Network & Endpoint Security Standard (Policy 28).

## 9. Retention & Disposal

- Data is retained only as long as legally or operationally required, per the Records Management & Retention Schedule (Policy 26) and Privacy Policy (04).
- Disposal renders data unrecoverable (cryptographic erasure, secure wipe to NIST 800-88, or physical destruction).

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Information classification | ISO 27001 A.5.12; SOC 2 C1.1 |
| Labelling of information | ISO 27001 A.5.13 |
| Protection / handling of assets | ISO 27001 A.8.10–A.8.12; SOC 2 C1.1–C1.2 |
| Secure disposal | ISO 27001 A.7.14, A.8.10; PCI-DSS Req. 9.4 |
| DLP / data leakage prevention | ISO 27001 A.8.12 |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the GRC / exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CISO and DPO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| % Restricted/Confidential repositories with encryption | 100% | Quarterly | CISO |
| DLP policy violations (Restricted) | Trend ↓ | Monthly | Security |
| % assets with assigned owner & classification | ≥ 95% | Quarterly | Data Owners |
| Secure-disposal certificates retained | 100% | Quarterly | IT |

## 13. Related Documents

- Data Privacy & Protection Policy (04)
- Access Control Policy (02)
- Cryptography & Key Management (11)
- Records Management & Retention Schedule (Policy 26)
- PCI-DSS Policy (14)
- Data Retention & Backup Standard (see Policy Index)

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
