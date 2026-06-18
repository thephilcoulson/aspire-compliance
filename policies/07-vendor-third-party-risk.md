# 7 — Vendor & Third-Party Risk Management Policy

| | |
|---|---|
| **Document ID** | POL-07 |
| **Policy Owner** | CISO / Procurement / Compliance |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022 (A.5.19–A.5.23); SOC 2; MAS Guidelines on Outsourcing |

---

## 1. Purpose

To manage risks arising from third parties and outsourcing arrangements, ensuring vendors meet Aspire's security, privacy, resilience, and regulatory requirements throughout the relationship lifecycle. As a regulated fintech relying on cloud, payment, and data providers, third-party risk is a primary source of Aspire's operational and compliance risk.

## 2. Scope

All third parties that process Company or customer data, provide material or critical services, or connect to Company systems — including SaaS, cloud (IaaS/PaaS), payment partners, sponsor/partner banks, KYC/AML data providers, and their sub-processors. Material outsourcing is additionally governed by the Outsourcing & Cloud Governance Standard (see Policy Index).

## 3. Definitions & Glossary

| Term | Definition |
|------|------------|
| **Outsourcing** | An arrangement where a third party performs a function that Aspire could otherwise perform itself. |
| **Material Outsourcing** | Outsourcing whose failure could materially affect Aspire's operations, customers, or compliance (per MAS Guidelines on Outsourcing). |
| **Sub-processor** | A third party engaged by a vendor to process Aspire data. |
| **DPA** | Data Processing Agreement. |
| **AOC / SOC report** | Attestation of Compliance / Service Organisation Control report evidencing a vendor's controls. |
| **Concentration risk** | Over-reliance on a single provider or location. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| CISO | Owns the third-party security risk framework. |
| Vendor Risk / TPRM | Runs tiering, due diligence, and ongoing monitoring. |
| Procurement | Manages sourcing and contract execution. |
| Legal | Drafts and negotiates security, DPA, audit, and exit clauses. |
| Business Owner | Owns the relationship and the residual risk. |
| Compliance | Confirms regulatory (outsourcing/AML) requirements are met. |

### 4.1 RACI — Vendor Lifecycle

| Activity | CISO | Vendor Risk | Procurement | Legal |
|---|---|---|---|---|
| Tier vendors by risk | A | R | C | I |
| Conduct due diligence | A | R | C | C |
| Negotiate security/DPA clauses | C | C | R | A |
| Ongoing monitoring & reassessment | A | R | C | I |
| Offboard vendors securely | A | R | C | I |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Risk-Based Tiering

| Tier | Criteria | Diligence |
|---|---|---|
| Critical / Material | Access to Restricted data or critical/material service dependency | Full security & financial due diligence; SOC 2/ISO/PCI evidence; contract + SLA; board/regulator notification where required; exit plan |
| High | Access to Confidential/personal data | Security questionnaire; certification review; DPA; annual reassessment |
| Standard | Limited/no sensitive data | Baseline review; lightweight reassessment |

## 6. Due Diligence (Procedure)

- Assess security posture (ISO 27001, SOC 2, PCI-DSS as relevant), financial stability, regulatory standing, data-handling, sub-processors, and resilience.
- For payment/financial outsourcing, ensure compliance with the MAS Guidelines on Outsourcing (and equivalent local rules): risk assessment, ability to monitor, audit and access rights, data confidentiality, and a viable exit strategy.

## 7. Contracts

Contracts with in-scope vendors must include: confidentiality and data protection (DPA where personal data is processed); security control requirements and right to audit; breach-notification obligations and timelines; sub-processor controls and prior notice; service levels; business-continuity commitments; and exit/termination and data-return/destruction provisions.

## 8. Ongoing Monitoring

- Periodic reassessment by tier (Critical/Material: annual; High: annual/biennial).
- Track certification renewals, SOC reports, security incidents, SLA performance, and adverse media.
- Maintain a current vendor inventory and an up-to-date sub-processor list.

## 9. Offboarding & Concentration Risk

- On exit, ensure secure return or destruction of Company data and revocation of access.
- Identify critical-service concentration; maintain continuity and exit plans for key dependencies (Policy 09; Outsourcing Standard the relevant policy).

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Supplier relationship security policy | ISO 27001 A.5.19 |
| Addressing security in supplier agreements | ISO 27001 A.5.20; SOC 2 CC9.2 |
| ICT supply chain security | ISO 27001 A.5.21 |
| Monitoring & review of supplier services | ISO 27001 A.5.22; SOC 2 CC9.2 |
| Cloud service security | ISO 27001 A.5.23 |
| Material outsourcing governance | MAS Guidelines on Outsourcing §5–§7 |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the GRC / exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CISO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| % critical vendors with current due diligence | 100% | Quarterly | Vendor Risk |
| % in-scope vendors with executed DPA | 100% | Quarterly | Legal |
| Vendor reassessments completed on schedule | ≥ 95% | Quarterly | Vendor Risk |
| Open vendor risk findings past due | 0 | Monthly | Vendor Risk |

## 13. Related Documents

- Outsourcing & Cloud Governance Standard (see Policy Index)
- Data Privacy & Protection (04)
- Business Continuity & DR (09)
- Information Security Policy (01)
- Procurement & Supplier Code of Conduct (see Policy Index)
- Vendor Inventory; Sub-processor List

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
