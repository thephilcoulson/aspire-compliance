# 32 — Data Retention & Backup Standard

| | |
|---|---|
| **Document ID** | POL-32 |
| **Policy Owner** | Chief Information Security Officer / Head of IT |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard / Regime** | ISO/IEC 27001:2022 (A.8.13–A.8.14); SOC 2 Availability; PCI-DSS; MAS TRM |

---

## 1. Purpose

To define technical requirements for backing up Aspire's critical data and systems and for retaining/disposing of data in line with the Records Management schedule and recovery objectives, ensuring data can be restored after loss or corruption.

## 2. Scope

All critical data, databases, configurations, and systems required to operate and recover Aspire's services.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| Backup | A copy of data for recovery purposes. |
| RPO | Recovery Point Objective (max tolerable data loss). |
| RTO | Recovery Time Objective (max tolerable downtime). |
| Immutable Backup | A backup that cannot be altered/deleted within a window. |
| Restore Test | A validation that backups can be recovered. |
| Air-gap / Isolation | Separation protecting backups from compromise. |
| Retention Tier | A defined backup keep-period. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| CISO / Head of IT | Owns backup strategy and recovery objectives. |
| Platform / IT Operations | Configures and runs backups and restores. |
| Data Owners | Define criticality, RPO/RTO, and retention. |
| Internal Audit | Reviews backup integrity and testing. |

### 4.1 RACI

| Activity | CISO/IT Head | IT Ops | Data Owners | Internal Audit |
|---|---|---|---|---|
| Define backup scope & RPO/RTO | A | C | R | I |
| Operate backups | A | R | I | I |
| Test restores | A | R | C | C |
| Enforce retention/disposal | A | R | R | I |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Backup Scope & Objectives

Critical data and systems are identified via the BIA (Policy 09) and assigned recovery objectives. Indicative tiers:
- **Tier 1 (critical, e.g. ledger/payments): RTO 4 hours, RPO 15 minutes.**
- **Tier 2 (important): RTO 24 hours, RPO 4 hours.**
- **Tier 3 (standard): RTO 72 hours, RPO 24 hours.**
Objectives are confirmed per system.

## 6. Backup Configuration

Backups are encrypted (AES-256), access-controlled, and stored in geographically separate locations. Immutable/air-gapped copies protect against ransomware. Backup schedules meet the defined RPO for each tier.

## 7. Restore Testing

Restoration is tested at least **quarterly** for critical systems to validate integrity and confirm RTO/RPO are met; test results, gaps, and corrective actions are documented and tracked (Policy 09).

## 8. Retention & Disposal

Backup retention aligns with the Records Management schedule (Policy 26) and privacy storage-limitation obligations (Policy 04). Personal-data deletion accounts for backup cycles, with documented timelines for backup expiry. Expired backups are securely destroyed.

## 9. Monitoring & Alerting

Backup jobs are monitored; failures alert IT Operations and are remediated promptly. Backup success/failure metrics are reported.

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Information backup | ISO 27001 A.8.13; SOC 2 A1.2 |
| Redundancy of facilities | ISO 27001 A.8.14; SOC 2 A1.2 |
| Recovery objectives & testing | ISO 22301 (aligned); MAS TRM |
| Retention alignment | PDPA Retention Limitation; FATF Rec. 11 |

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
| Backup success rate | ≥ 99% | Weekly | IT Ops |
| Restore tests passed (critical) | 100% | Quarterly | IT Ops |
| Critical systems meeting RPO in tests | 100% | Quarterly | IT Ops |
| Expired backups disposed on schedule | 100% | Quarterly | IT Ops |

## 13. Related Documents

- Business Continuity & DR (09)
- Records Management & Retention (26)
- Data Privacy & Protection (04)
- Cryptography & Key Management (11)
- Data Classification & Handling (03)

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
