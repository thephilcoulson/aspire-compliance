# 9 — Business Continuity & Disaster Recovery Policy

| | |
|---|---|
| **Document ID** | POL-09 |
| **Policy Owner** | COO / CISO |
| **Approved By** | Executive / Board |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual (+ post-test) |
| **Classification** | Internal |
| **Aligned Standard** | ISO 22301 (aligned); SOC 2 Availability; MAS Business Continuity Guidelines |

---

## 1. Purpose

To ensure Aspire can continue or rapidly resume critical operations during and after a disruptive event, protecting customers' access to their funds and services, staff, and regulatory obligations. Continuity of payment and account services is a regulatory and reputational imperative for a fintech.

## 2. Scope

All critical business functions, supporting systems and infrastructure, facilities, people, and critical third parties (including cloud and partner banks).

## 3. Definitions & Glossary

| Term | Definition |
|------|------------|
| **BIA** | Business Impact Analysis — identifies critical processes and their tolerances. |
| **RTO** | Recovery Time Objective — maximum tolerable downtime. |
| **RPO** | Recovery Point Objective — maximum tolerable data loss. |
| **MTPD** | Maximum Tolerable Period of Disruption. |
| **DR** | Disaster Recovery — technical recovery of systems and data. |
| **Failover** | Switching to a standby system/site. |
| **Crisis Management** | Senior coordination of a major disruptive event. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| BCP Coordinator | Maintains plans, BIA, and the exercise schedule. |
| Recovery Teams | Execute documented recovery procedures. |
| IT / Engineering | Operate backups, redundancy, and failover. |
| Executive Sponsor / Crisis Lead | Activation decisions and external communications. |
| Business Owners | Provide BIA inputs and validate workarounds. |

### 4.1 RACI — Continuity Lifecycle

| Activity | BCP Coordinator | Recovery Teams | IT/Eng | Exec Sponsor |
|---|---|---|---|---|
| Maintain Business Impact Analysis | A | R | C | I |
| Define RTO/RPO per service | A | R | C | I |
| Operate backups & DR | C | R | A | I |
| Run BCP/DR exercises | A | R | C | C |
| Activate crisis management | A | C | C | R |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Business Impact Analysis (Procedure)

- Identify critical processes and dependencies (systems, people, vendors, data).
- Define **RTO** and **RPO** for each critical service; record the MTPD.
- Maintain a current BIA register reviewed at least annually and on material change.

## 6. Continuity Strategies

- Redundancy and resilience for critical infrastructure (multi-AZ/region as appropriate).
- Documented manual workarounds for key processes.
- Remote-capable alternate work arrangements for staff.
- Continuity provisions and exit plans for critical vendors (Policy 07; Outsourcing Standard the relevant policy).

## 7. Backup & Data Recovery

- Critical data is backed up per defined schedule; backups are encrypted, access-controlled, and immutable where feasible (ransomware resilience).
- Backups are stored in geographically separate locations.
- Restoration is tested periodically to validate integrity and meet RPO (see Data Retention & Backup Standard the relevant policy).

## 8. Disaster Recovery

DR plans and runbooks are maintained for critical systems; failover/recovery procedures are documented, owned, and tested.

## 9. Crisis Management & Communications

A crisis management team and escalation tree are defined; communication plans cover staff, customers, regulators, partners, and media, with pre-approved templates.

## 10. Testing & Exercises

BCP/DR is tested at least annually (tabletop and/or technical failover); results, gaps, and corrective actions are documented and tracked to closure.

## 11. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| ICT readiness for business continuity | ISO 27001 A.5.30; ISO 22301 Cl. 8 |
| Information security during disruption | ISO 27001 A.5.29 |
| Redundancy of processing facilities | ISO 27001 A.8.14; SOC 2 A1.2 |
| Backup | ISO 27001 A.8.13; SOC 2 A1.2 |
| Business impact analysis & strategy | ISO 22301 Cl. 8.2–8.3; MAS BCM |
| Exercising & testing | ISO 22301 Cl. 8.5 |

## 12. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the GRC / exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 13. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the COO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| Critical services meeting RTO in tests | 100% | Per test | BCP Coordinator |
| Backup restoration tests passed | 100% | Quarterly | IT |
| BCP/DR exercises completed | ≥ 1/yr | Annual | BCP Coordinator |
| Open continuity findings past due | 0 | Monthly | BCP Coordinator |

## 14. Related Documents

- Vendor & Third-Party Risk (07)
- Incident Response (08)
- Data Retention & Backup Standard (see Policy Index)
- Outsourcing & Cloud Governance (Policy 27)
- Operational Risk & Regulatory Reporting (see Policy Index)
- BIA Register; DR Runbooks

## 15. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
