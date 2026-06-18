# 19 — Fraud Risk Management

| | |
|---|---|
| **Document ID** | POL-19 |
| **Policy Owner** | Head of Fraud / Financial Crime |
| **Approved By** | Audit & Risk Committee |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal — Restricted |
| **Aligned Standard / Regime** | MAS guidance on fraud; ISO 37001 (aligned); enterprise risk |

---

## 1. Purpose

To prevent, detect, investigate, and respond to internal and external fraud affecting Aspire, its customers, and partners — including account takeover, payment fraud, application/onboarding fraud, authorised push payment scams, and internal fraud — protecting customer funds and Aspire's financial integrity.

## 2. Scope

All products, channels, customers, employees, and partners; all fraud typologies relevant to a business-finance platform.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| Fraud | Intentional deception for unlawful gain. |
| ATO | Account Takeover — unauthorised control of a customer account. |
| APP Scam | Authorised Push Payment scam — customer tricked into paying a fraudster. |
| Application Fraud | Fraud at onboarding (synthetic/stolen identity). |
| First-party Fraud | Fraud by the genuine customer (e.g. chargeback abuse). |
| Internal Fraud | Fraud by staff/insiders. |
| Mule Account | An account used to launder/move fraud proceeds. |
| Fraud Loss | Financial loss attributable to fraud. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| Head of Fraud | Owns the fraud risk framework and strategy. |
| Fraud Operations | Runs detection, rules, and case investigation. |
| Engineering / Data Science | Builds detection models and controls. |
| Customer Support | First contact for reported fraud; follows playbooks. |
| Internal Audit / HR | Handle internal-fraud investigations. |

### 4.1 RACI

| Activity | Head of Fraud | Fraud Ops | Eng/DS | Audit/HR |
|---|---|---|---|---|
| Maintain fraud risk assessment & typologies | A | R | C | I |
| Operate detection rules/models | A | R | R | I |
| Investigate & resolve fraud cases | A | R | C | C |
| Recover funds & manage chargebacks | A | R | I | C |
| Report internal fraud | C | R | I | A |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Fraud Risk Assessment & Typologies

Maintain a fraud risk assessment covering each product/channel and the relevant typologies (ATO, APP scams, application/synthetic-identity fraud, card fraud, mule activity, internal fraud). Controls are calibrated to assessed risk and refreshed on emerging typologies.

## 6. Prevention Controls

Layered preventive controls: device fingerprinting, behavioural biometrics, step-up authentication, velocity and limit controls, payee verification, onboarding identity checks (Policy 13), and segregation of duties for internal processes.

## 7. Detection & Monitoring

Real-time and near-real-time detection using rules and machine-learning models, with feedback loops from confirmed cases. Suspicious activity that may also be money laundering is referred to AML for STR consideration (Policy 12) — fraud and AML operate jointly but distinctly.

## 8. Case Management & Investigation Procedure

1. Detect/report (alert, customer report, or partner notice).
2. Triage and prioritise by loss/risk.
3. Investigate, gather evidence, and decide action (block, recover, close).
4. Customer remediation/communication.
5. Recovery (recall funds, chargebacks) and root-cause feedback to controls.

## 9. Internal Fraud

Internal fraud is handled confidentially with HR, Legal, and Internal Audit; segregation of duties and access controls (Policy 02) are primary preventive controls; whistleblowing (Policy the relevant policy) is a key detection channel.

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Fraud risk management framework | MAS fraud-management expectations; enterprise risk |
| Fraud detection & monitoring | SOC 2 CC7.2 (aligned); internal controls |
| Segregation of duties (internal fraud) | ISO 27001 A.5.3 |
| Linkage to AML reporting | FATF Rec. 20; MAS PSN01 §9 |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the the GRC exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the Head of Fraud and ARC and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| Fraud loss rate (bps of volume) | ≤ 95% | Monthly | Head of Fraud |
| Fraud detection rate / recall | ≥ 95% | Monthly | Fraud Ops |
| Case resolution within SLA | ≥ 95% | Monthly | Fraud Ops |
| Funds recovered / blocked | Tracked | Monthly | Fraud Ops |

## 13. Related Documents

- AML/CFT Policy (12)
- Transaction Monitoring Standard (Policy 20)
- Incident Response (08)
- Whistleblowing & Speak-Up (Policy 25)
- Customer Onboarding & Account Lifecycle Compliance (Policy 37)
- Fraud Risk Assessment

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
