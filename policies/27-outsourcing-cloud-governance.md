# 27 — Outsourcing & Cloud Governance

| | |
|---|---|
| **Document ID** | POL-27 |
| **Policy Owner** | CCO / CISO |
| **Approved By** | Board / Audit & Risk Committee |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard / Regime** | MAS Guidelines on Outsourcing; MAS Cloud advisories; ISO 27017; SOC 2 |

---

## 1. Purpose

To govern outsourcing and cloud-service arrangements in line with the MAS Guidelines on Outsourcing and cloud advisories, ensuring Aspire retains accountability, manages risk and resilience, and preserves audit and access rights when relying on third parties — especially for material/critical functions.

## 2. Scope

All outsourcing and cloud arrangements (IaaS/PaaS/SaaS), with heightened controls for material outsourcing supporting regulated activities.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| Outsourcing | A third party performing a function Aspire could perform itself. |
| Material Outsourcing | Outsourcing whose failure could materially affect operations/customers/compliance. |
| Cloud Service | On-demand computing from a cloud provider. |
| Shared Responsibility | The split of security duties between Aspire and the cloud provider. |
| Sub-outsourcing | A service provider's own outsourcing. |
| Exit Plan | A documented plan to migrate away from a provider. |
| Audit/Access Rights | Contractual rights to audit/inspect a provider. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| CCO / CISO | Co-own outsourcing/cloud governance and material-outsourcing register. |
| Cloud / Platform Engineering | Implements secure cloud configuration and shared-responsibility controls. |
| Vendor Risk | Performs due diligence and ongoing monitoring (Policy 07). |
| Legal | Ensures audit/access, sub-outsourcing, and exit clauses. |
| Board / ARC | Approves material outsourcing; notified per regulatory rules. |

### 4.1 RACI

| Activity | CCO/CISO | Cloud Eng | Vendor Risk | Legal | Board |
|---|---|---|---|---|---|
| Classify outsourcing materiality | A | C | R | C | I |
| Approve material outsourcing | C | C | C | C | A |
| Secure cloud configuration | A | R | C | I | I |
| Maintain exit & continuity plans | A | R | C | C | I |
| Monitor providers & sub-outsourcing | A | C | R | C | I |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Materiality Assessment

Each arrangement is assessed for materiality using impact on operations, customers, compliance, and recovery. Material outsourcing follows enhanced governance: documented risk assessment, board/ARC approval, regulator notification where required, audit/access rights, data confidentiality, business-continuity assurance, and a viable exit strategy (MAS Guidelines on Outsourcing).

## 6. Cloud Security & Shared Responsibility

Cloud usage follows a documented shared-responsibility model: the provider secures the cloud; Aspire secures its configuration, identities, data, and workloads. Baselines cover secure landing zones, IAM (Policy the relevant policy), encryption (Policy 11), network controls (Policy the relevant policy), logging (Policy the relevant policy), and CSPM/posture management. Data-residency requirements are enforced per market.

## 7. Due Diligence & Contracts

Providers undergo due diligence (Policy 07); contracts include security requirements, audit/access rights (including for the regulator), breach notification, sub-outsourcing controls and prior notice, data return/destruction, SLAs, and termination/exit provisions.

## 8. Concentration, Sub-outsourcing & Resilience

Concentration risk (single provider/region) is assessed and mitigated; material sub-outsourcing requires notice and assessment; resilience is validated against RTO/RPO (Policy 09).

## 9. Exit & Continuity Planning

Each material arrangement has a documented, tested exit plan covering data portability, alternative providers, and stand-up timelines to avoid lock-in and ensure continuity.

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Outsourcing governance & materiality | MAS Guidelines on Outsourcing §4–§5 |
| Audit/access & regulator rights | MAS Guidelines on Outsourcing §5.6 |
| Cloud security controls | ISO 27017; ISO 27001 A.5.23; SOC 2 CC9.x |
| Business continuity & exit | MAS Outsourcing §5.9; ISO 22301 (aligned) |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the the GRC exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CCO and Board and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| Material outsourcing with board approval | 100% | Per arrangement | CCO |
| Cloud posture (CSPM) critical findings open | 0 | Weekly | Cloud Eng |
| Material arrangements with tested exit plans | 100% | Annual | CISO |
| Provider monitoring completed on schedule | ≥ 95% | Quarterly | Vendor Risk |

## 13. Related Documents

- Vendor & Third-Party Risk (07)
- Business Continuity & DR (09)
- Network & Endpoint Security Standard (Policy 28)
- Logging, Monitoring & SIEM Standard (Policy 29)
- Identity & Access Management Standard (see Policy Index)
- Material Outsourcing Register

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
