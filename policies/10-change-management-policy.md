# 10 — Change Management Policy

| | |
|---|---|
| **Document ID** | POL-10 |
| **Policy Owner** | CTO / Head of Engineering |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | SOC 2 (Change Management); ISO/IEC 27001:2022 (A.8.32); PCI-DSS Req. 6 |

---

## 1. Purpose

To ensure changes to production systems, applications, configurations, and infrastructure are made in a controlled, secure, tested, and auditable manner, minimising risk to the availability, integrity, and security of Aspire's financial platform.

## 2. Scope

All changes to production systems, code, configurations, data schemas, and infrastructure (including infrastructure-as-code), and emergency changes.

## 3. Definitions & Glossary

| Term | Definition |
|------|------------|
| **Change** | Any addition, modification, or removal affecting a production service. |
| **Standard change** | A pre-approved, low-risk, repeatable change. |
| **Normal change** | A change requiring review, testing, and approval. |
| **Emergency change** | An urgent change to restore service or patch a critical vulnerability. |
| **CAB** | Change Advisory Board (where applicable). |
| **Rollback** | A planned reversion to a prior known-good state. |
| **SoD** | Segregation of Duties between development and production deployment. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| CTO / Head of Engineering | Owns the change framework and CI/CD controls. |
| Change Owner / Requester | Documents the change, rationale, and rollback. |
| Reviewer / Approver / CAB | Reviews risk and authorises the change. |
| Release / DevOps | Executes controlled deployment. |
| Security | Ensures security gates (SAST/DAST/dependency scans) are enforced. |

### 4.1 RACI — Change Lifecycle

| Activity | Engineer | Reviewer | CAB/Approver | Change Owner |
|---|---|---|---|---|
| Raise change request | R | I | C | A |
| Peer review / approve change | C | R | A | I |
| Test change | R | C | I | A |
| Deploy to production | R | A | I | I |
| Approve emergency change (retrospective) | C | A | R | I |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Change Principles

- **Authorised:** Every change is reviewed and approved before deployment.
- **Tested:** Changes are tested prior to production release.
- **Traceable:** Changes are tracked from request through deployment to verification.
- **Segregation of duties:** Developers cannot unilaterally approve and deploy their own production changes where feasible; enforced via branch protection and pipeline gates.

## 6. Change Categories

| Type | Definition | Approval |
|---|---|---|
| Standard | Pre-approved, low-risk, repeatable | Pre-authorised |
| Normal | Requires review/testing | Reviewer / CAB |
| Emergency | Urgent fix or critical patch | Expedited approval + retrospective review |

## 7. Change Process (Procedure)

1. **Request** — documented in the change/ticketing system with rationale, risk, and rollback plan.
2. **Review & Approve** — peer review (code review/PR) and approval by an authorised approver.
3. **Test** — automated and/or manual testing in non-production.
4. **Deploy** — via controlled CI/CD pipeline; production access restricted and logged.
5. **Verify** — post-deployment validation and monitoring.
6. **Document** — record outcome and link evidence to the change record.

## 8. Secure Development Integration

- Security requirements are integrated into the SDLC (see SSDLC Standard the relevant policy).
- Code is peer-reviewed; secrets are not committed to source control (secret scanning enforced).
- Automated security testing (SAST/DAST/SCA/dependency scanning) runs in the pipeline.
- Separate development, staging, and production environments with controlled promotion.

## 9. Emergency Changes

May bypass standard lead times but require approval (verbal/expedited) and full retrospective documentation and review within defined SLA.

## 10. Rollback

Every change includes a rollback or recovery plan; deployments prefer progressive techniques (canary/blue-green) where feasible.

## 11. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Change management | ISO 27001 A.8.32; SOC 2 CC8.1 |
| Separation of environments | ISO 27001 A.8.31 |
| Secure development lifecycle | ISO 27001 A.8.25–A.8.30; PCI-DSS Req. 6.2–6.3 |
| Segregation of duties | ISO 27001 A.5.3; SOC 2 CC8.1 |
| Security testing in development | ISO 27001 A.8.29; PCI-DSS Req. 6.3 |

## 12. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the GRC / exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 13. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CTO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| % production changes via approved pipeline | 100% | Monthly | Eng |
| Change failure rate | ≤ 95% | Monthly | Eng |
| Unauthorised changes detected | 0 | Monthly | Security |
| Emergency changes with retrospective review | 100% | Monthly | Change Owner |

## 14. Related Documents

- Secure Software Development Lifecycle Standard (see Policy Index)
- Vulnerability & Patch Management Standard (see Policy Index)
- Information Security Policy (01)
- PCI-DSS Policy (14)
- Logging, Monitoring & SIEM Standard (Policy 29)

## 15. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
