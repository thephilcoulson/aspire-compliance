# 8 — Incident Response & Breach Management Policy

| | |
|---|---|
| **Document ID** | POL-08 |
| **Policy Owner** | CISO / Head of Security |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual (+ post-incident) |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022 (A.5.24–A.5.28); SOC 2; PDPA/GDPR breach rules; MAS TRM |

---

## 1. Purpose

To ensure security and data-breach incidents are detected, reported, triaged, contained, eradicated, and resolved promptly, with appropriate forensic preservation and regulatory/customer notification. Given Aspire's role handling customer funds and data, timely and effective incident response is critical to customer trust and regulatory standing (MAS incident-reporting expectations, PDPA/GDPR breach rules).

## 2. Scope

All security incidents affecting Company systems, data, or services, including incidents originating at third parties and affecting Aspire data or operations.

## 3. Definitions & Glossary

| Term | Definition |
|------|------------|
| **Event** | An observable occurrence in a system or network. |
| **Incident** | An event that compromises (or threatens) the CIA of information or services. |
| **Data Breach** | Unauthorised access, disclosure, loss, or alteration of personal/regulated data. |
| **SEV** | Severity level assigned to an incident. |
| **IC** | Incident Commander — owns coordination of a response. |
| **IOC** | Indicator of Compromise. |
| **RCA** | Root-Cause Analysis. |
| **Chain of custody** | Documented handling of evidence to preserve its integrity. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| Incident Commander | Owns coordination and decision-making during an incident. |
| Security Team | Technical investigation, containment, eradication, recovery. |
| Legal / Compliance | Regulatory and legal obligations; notification review. |
| DPO | Personal-data breach risk assessment and PDPC/SA notification. |
| Communications | Internal and external messaging. |
| Executive Sponsor | Escalation, resourcing, and approvals. |

### 4.1 RACI — Incident Lifecycle

| Activity | Security Team | Incident Commander | Legal/DPO | Exec Sponsor |
|---|---|---|---|---|
| Detect & report incidents | R | A | C | I |
| Triage & classify severity | R | A | C | I |
| Contain, eradicate, recover | R | A | C | I |
| Regulatory/customer notification decision | C | A | R | C |
| Post-incident review & actions | R | A | C | C |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Severity Classification

| Severity | Description | Example | Target Response |
|---|---|---|---|
| SEV1 (Critical) | Major impact; data breach or service outage | Confirmed exfiltration of customer PII; payment outage | Immediate; 24/7 mobilisation |
| SEV2 (High) | Significant but contained | Malware on a server; limited exposure | ≤ 1 hour acknowledgement |
| SEV3 (Medium) | Limited impact | Single compromised low-priv account | ≤ 4 hours |
| SEV4 (Low) | Minimal impact | Isolated policy violation | Next business day |

## 6. Response Lifecycle (Procedure)

1. **Detect & Report** — anyone aware of an incident reports it immediately via channel; 24/7 reporting available; SIEM/EDR alerts feed the same queue (see Policy Index).
2. **Triage & Classify** — Security assesses severity and activates the response team.
3. **Contain** — isolate affected systems; preserve evidence; prevent spread.
4. **Eradicate** — remove the root cause (malware, access, vulnerability).
5. **Recover** — restore services securely; validate integrity; monitor for recurrence.
6. **Post-Incident Review** — RCA and corrective actions tracked to closure within defined SLA.

## 7. Regulatory & Customer Notification

- **PDPA:** Notify the PDPC and affected individuals where a breach meets notifiable thresholds (significant harm / scale), within statutory timeframes.
- **GDPR:** Notify the supervisory authority within 72 hours where required; notify data subjects for high-risk breaches.
- **Financial regulators:** Notify per applicable obligations (e.g. MAS incident reporting timelines for relevant incidents).
- **Card data:** Follow PCI-DSS and card-scheme/acquirer breach procedures (Policy 14).
- All notification decisions are documented, legally reviewed, and time-stamped.

## 8. Evidence & Forensics

Preserve logs and evidence with documented chain of custody for potential investigation or legal proceedings; engage external DFIR specialists where warranted.

## 9. Testing & Readiness

Incident response plans, runbooks, and on-call rosters are maintained and tested at least annually (tabletop and/or simulation), including a personal-data-breach scenario and a third-party-incident scenario.

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Incident management planning | ISO 27001 A.5.24; SOC 2 CC7.3 |
| Assessment & decision on events | ISO 27001 A.5.25; SOC 2 CC7.4 |
| Response to incidents | ISO 27001 A.5.26; SOC 2 CC7.4–CC7.5 |
| Learning from incidents | ISO 27001 A.5.27 |
| Collection of evidence | ISO 27001 A.5.28 |
| Breach notification | PDPA Part 6A; GDPR Art. 33–34 |

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
| Mean time to detect (MTTD) | ≤ target | Monthly | Security |
| Mean time to contain (MTTC) | ≤ target | Monthly | Security |
| Notifications made within statutory deadline | 100% | Per event | Legal/DPO |
| Post-incident actions closed on time | ≥ 95% | Monthly | Security |
| IR exercises completed | ≥ 1/yr | Annual | CISO |

## 13. Related Documents

- Information Security Policy (01)
- Data Privacy & Protection (04)
- PCI-DSS Policy (14)
- Business Continuity & DR (09)
- Logging, Monitoring & SIEM Standard (Policy 29)
- Fraud Risk Management (Policy 19)
- Operational Risk & Regulatory Reporting (see Policy Index)
- Incident Runbooks; On-call Roster

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
