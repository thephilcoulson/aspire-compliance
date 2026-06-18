# 26 — Records Management & Retention Schedule

| | |
|---|---|
| **Document ID** | POL-26 |
| **Policy Owner** | General Counsel / DPO |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard / Regime** | PDPA; MAS/FATF record-keeping; ISO 15489 (aligned); SOC 2 |

---

## 1. Purpose

To ensure Aspire's records are created, stored, retained, and disposed of in line with legal, regulatory, and operational requirements — meeting AML, tax, privacy, and evidentiary obligations while avoiding over-retention of personal data.

## 2. Scope

All business records in any format (electronic, physical), across all functions, systems, and markets.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| Record | Information created/received as evidence of an activity. |
| Retention Period | The minimum/maximum time a record must be kept. |
| Retention Schedule | The master list of record types and their periods. |
| Legal Hold | A suspension of disposal due to litigation/investigation. |
| Disposition | Final action on a record (destroy/archive/transfer). |
| Vital Record | A record essential to operations/recovery. |
| Defensible Disposal | Documented, policy-driven destruction. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| General Counsel / DPO | Owns the retention schedule and legal holds. |
| Records / Information Mgmt | Maintains schedules and disposal processes. |
| Function Owners | Apply retention to their records. |
| IT | Implements retention/disposal in systems and backups. |

### 4.1 RACI

| Activity | GC/DPO | Records Mgmt | Functions | IT |
|---|---|---|---|---|
| Maintain retention schedule | A | R | C | C |
| Apply retention to records | C | C | R | A |
| Execute defensible disposal | A | R | C | R |
| Apply & release legal holds | A | R | I | C |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Retention Schedule (Illustrative)

The master retention schedule defines periods by record type, for example:
- KYC/CDD and AML records: **≥ 5 years** after relationship ends (FATF Rec. 11; MAS PSN01).
- Transaction records: **≥ 5 years**.
- Tax records (incl. FATCA/CRS): per local tax law (commonly **5–7 years**).
- Employment records: per labour law.
- Personal data: only as long as necessary for the purpose (PDPA storage limitation).
Actual periods are set per jurisdiction and recorded in the schedule (the figures above are placeholders to be confirmed).

## 6. Storage & Integrity

Records are stored in approved systems with access controls, classification (Policy 03), integrity protection, and (for vital records) backup and recovery (Policy the relevant policy). Original/evidential records maintain authenticity and chain of custody where needed.

## 7. Retention & Disposal Procedure

1. Classify the record and map it to a retention period.
2. Retain in an approved repository.
3. On expiry, and absent a legal hold, dispose defensibly (secure deletion/destruction per Policy 03).
4. Record the disposition.
Over-retention of personal data beyond its purpose is prohibited.

## 8. Legal Holds

On notice of litigation, investigation, or regulatory request, affected records are placed on legal hold and exempted from disposal until the hold is formally released by Legal.

## 9. Backups & Personal Data

Backup retention is aligned with the schedule and privacy obligations; personal-data deletion processes account for backup cycles and document the timeline for backup expiry (Policy the relevant policy).

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Record keeping (AML) | FATF Rec. 11; MAS PSN01 §10 |
| Storage limitation (privacy) | PDPA Retention Limitation; GDPR Art. 5(1)(e) |
| Records management | ISO 15489 (aligned); SOC 2 CC2.0 |
| Defensible disposal | ISO 27001 A.8.10; PCI-DSS Req. 9.4 |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the the GRC exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the GC and DPO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| Records mapped to retention schedule | ≥ 95% | Quarterly | Records Mgmt |
| Over-retained personal data remediated | Trend ↓ | Quarterly | DPO |
| Legal holds applied within SLA | 100% | Per event | Legal |
| Defensible disposals logged | 100% | Quarterly | Records Mgmt |

## 13. Related Documents

- Data Classification & Handling (03)
- Data Privacy & Protection (04)
- AML/CFT Policy (12)
- Data Retention & Backup Standard (Policy 32)
- Tax & FATCA/CRS Compliance (Policy 42)
- Master Retention Schedule

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
