# 34 — AI Governance & Responsible Use

| | |
|---|---|
| **Document ID** | POL-34 |
| **Policy Owner** | Chief Technology Officer / CCO |
| **Approved By** | Executive / Board |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard / Regime** | ISO/IEC 42001 (aligned); NIST AI RMF; MAS FEAT principles; PDPA |

---

## 1. Purpose

To govern Aspire's development, procurement, and use of artificial intelligence and machine-learning systems so they are fair, accountable, transparent, secure, and compliant — including models used in fraud, AML, credit, and customer-facing features — and to control staff use of external AI tools.

## 2. Scope

All AI/ML systems built, bought, or used by Aspire, and all staff use of generative-AI and third-party AI tools with Company or customer data.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| AI/ML System | A system using machine learning or AI techniques. |
| Model Risk | Risk from model errors, bias, or misuse. |
| FEAT | Fairness, Ethics, Accountability, Transparency (MAS principles). |
| Explainability | Ability to understand/justify a model's outputs. |
| Human-in-the-loop | Human oversight of automated decisions. |
| Generative AI | AI producing text/code/media. |
| Model Inventory | The register of AI systems in use. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| CTO / CCO | Co-own AI governance and the model inventory. |
| Data Science / ML Eng | Build, validate, and monitor models. |
| Model Risk / Validation | Independently challenge and validate models. |
| Compliance / Legal / DPO | Ensure regulatory, fairness, and privacy compliance. |
| All Staff | Use approved AI tools within policy. |

### 4.1 RACI

| Activity | CTO/CCO | DS/ML | Model Risk | Compliance |
|---|---|---|---|---|
| Maintain AI model inventory | A | R | C | C |
| Validate models before deployment | A | C | R | C |
| Monitor models for drift/bias | A | R | R | C |
| Approve external AI tool use | A | C | I | R |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. AI Governance & Inventory

All AI/ML systems are recorded in a model inventory with purpose, owner, data used, risk tier, and oversight measures. Higher-risk uses (credit decisioning, AML/fraud scoring, customer-impacting automation) receive enhanced governance and human oversight.

## 6. Responsible-AI Principles (FEAT)

AI systems are designed for fairness (tested for unfair bias), ethics (legitimate purpose), accountability (named owner; human-in-the-loop for material decisions), and transparency (explainability proportionate to impact; customer disclosure where required), aligned to the MAS FEAT principles.

## 7. Model Development & Validation

Models are validated before deployment (performance, stability, bias, and security testing) and independently reviewed for higher-risk use. Training data is lawful, representative, and privacy-compliant (Policy 04). Models are monitored for drift and degradation, with retraining/rollback procedures.

## 8. Security of AI Systems

AI systems follow the SSDLC (Policy 31) and address AI-specific risks (prompt injection, data poisoning, model theft, sensitive-data leakage). Access to models and training data is controlled (Policy 02).

## 9. Staff Use of External AI Tools

Only sanctioned AI tools may process Company or customer data; Restricted/Confidential data must not be entered into unapproved external AI tools (Policy 05). Approved-tool usage follows data-handling and confidentiality requirements.

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| AI management system | ISO/IEC 42001 (aligned) |
| AI risk management | NIST AI RMF (aligned) |
| Fairness, ethics, accountability, transparency | MAS FEAT principles |
| Privacy in AI | PDPA; GDPR Art. 22 (automated decisions, where applicable) |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the the GRC exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CTO and Board and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| AI systems recorded in inventory | 100% | Quarterly | CTO |
| High-risk models independently validated | 100% | Per deployment | Model Risk |
| Models with drift/bias monitoring | 100% | Quarterly | DS/ML |
| Unsanctioned AI-tool data incidents | 0 | Monthly | Compliance |

## 13. Related Documents

- Acceptable Use Policy (05)
- Secure Software Development Lifecycle Standard (31)
- Data Privacy & Protection (04)
- Fraud Risk Management (19)
- Risk Management Policy (15)
- AI Model Inventory

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
