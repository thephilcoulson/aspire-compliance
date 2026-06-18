# 20 — Transaction Monitoring Standard

| | |
|---|---|
| **Document ID** | POL-20 |
| **Policy Owner** | MLRO |
| **Approved By** | Audit & Risk Committee |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal — Restricted |
| **Aligned Standard / Regime** | FATF Rec. 20; MAS Notice PSN01 §9; AML/CFT laws |

---

## 1. Purpose

To define how Aspire monitors customer transactions to detect, investigate, and report unusual or suspicious activity indicative of money laundering, terrorism financing, fraud, or sanctions evasion, with defined rules, typologies, thresholds, and service levels.

## 2. Scope

All customer transactions across all products (accounts, payments, cards, credit) and channels.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| Transaction Monitoring (TM) | Surveillance of transactions against rules/typologies. |
| Rule / Scenario | A configured pattern that generates alerts. |
| Threshold | A value/volume trigger for a rule. |
| Typology | A known pattern/method of financial crime. |
| Alert | A flagged transaction/behaviour requiring review. |
| Disposition | The documented outcome of an alert review. |
| SAR/STR | Suspicious Activity/Transaction Report. |
| Tuning | Adjusting rules/thresholds to balance detection and false positives. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| MLRO | Owns TM framework, rules governance, and reporting decisions. |
| TM Analysts | Investigate and disposition alerts. |
| TM Engineering / Data | Implements and tunes rules/models. |
| Model Risk / QA | Validates rules and tuning; quality-assures dispositions. |
| Internal Audit | Independent review of TM effectiveness. |

### 4.1 RACI

| Activity | MLRO | Analysts | TM Eng | Model QA | Internal Audit |
|---|---|---|---|---|---|
| Define & approve rules/typologies | A | C | R | C | I |
| Investigate & disposition alerts | A | R | I | C | I |
| Tune thresholds & reduce false positives | A | C | R | R | I |
| Escalate to STR | A | R | I | I | I |
| Independent TM effectiveness review | C | I | I | C | R |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Typologies Covered

Rules address relevant typologies including: structuring/smurfing; rapid movement / pass-through (mule) activity; round-amount and just-below-threshold transactions; unexpected high-velocity or high-value activity inconsistent with the customer profile; transactions to/from high-risk jurisdictions; dormant-then-active accounts; and trade-based and invoice-anomaly patterns relevant to business customers.

## 6. Rule Lifecycle & Governance

1. Propose rule with rationale and expected typology coverage.
2. Validate against historical data (back-testing).
3. Approve via MLRO/TM governance.
4. Deploy with documented threshold rationale.
5. Monitor performance (true/false positive rates) and tune at least quarterly.
All rule changes are version-controlled and auditable.

## 7. Alert Investigation & SLAs

Alerts are risk-prioritised and worked within SLA: high-priority within 1 business day, standard within 5 business days. Each disposition records the analyst, rationale, evidence reviewed, and outcome. Backlogs beyond SLA are escalated to the MLRO.

## 8. Escalation & Reporting

Alerts indicating suspicion are escalated to the MLRO for STR assessment (Policy 12). Fraud-indicative alerts are referred to Fraud (Policy the relevant policy); sanctions hits route to the sanctions process (Policy the relevant policy). Tipping-off is prohibited.

## 9. Quality Assurance & Model Validation

A QA program samples dispositions for accuracy and consistency; rules/models are independently validated periodically; coverage gaps and tuning decisions are documented and reported to the ARC.

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Monitoring of transactions | FATF Rec. 20; MAS PSN01 §9 |
| Risk-based scenario coverage | FATF Rec. 1; MAS PSN01 §4 |
| Record keeping of alerts/dispositions | FATF Rec. 11; MAS PSN01 §10 |
| Independent testing of TM | FATF Rec. 18; MAS PSN01 §12 |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the the GRC exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the MLRO and ARC and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| Alerts dispositioned within SLA | ≥ 95% | Weekly | MLRO |
| False-positive rate | ≤ 95% | Monthly | Model QA |
| Rules tuned on schedule | 100% | Quarterly | TM Eng |
| QA disposition accuracy | ≥ 95% | Monthly | Model QA |

## 13. Related Documents

- AML/CFT Policy (12)
- KYC/KYB Policy (13)
- Sanctions, Export Controls & Embargoes (18)
- Fraud Risk Management (19)
- PEP & EDD Procedure (see Policy Index)
- TM Rules Catalogue

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
