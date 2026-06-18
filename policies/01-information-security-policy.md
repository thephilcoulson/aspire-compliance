# 1 — Information Security Policy

| | |
|---|---|
| **Document ID** | POL-01 |
| **Policy Owner** | Chief Information Security Officer |
| **Approved By** | Board / Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022; SOC 2 |

---

## 1. Purpose

To establish, operate, maintain, and continually improve Aspire's Information Security Management System (ISMS), and to define the principles, responsibilities, and controls that protect the confidentiality, integrity, and availability (CIA) of information assets supporting Aspire's business-finance platform. This policy is the apex document of Aspire's security control framework and sets the mandate under which all subordinate security standards (Policies 02, 03, 05, 08, 10, 11, and the technical standards the relevant policy+) operate.

## 2. Scope

All information assets owned, controlled, or processed by Aspire — including customer data, KYC/KYB records, transaction and ledger data, cardholder data, source code, cryptographic material, infrastructure, SaaS services, and personnel — regardless of location, ownership of the device, or media (electronic, physical, or verbal). It applies to all employees, contractors, service accounts, and third parties with access to Aspire information or systems.

## 3. Definitions & Glossary

| Term | Definition |
|------|------------|
| **Asset** | Anything of value to Aspire, including information, systems, and services. |
| **CIA** | Confidentiality, Integrity, Availability — the core security objectives. |
| **ISMS** | Information Security Management System — the governance framework for security per ISO 27001. |
| **SoA** | Statement of Applicability — the documented set of Annex A controls Aspire applies and the justification. |
| **Threat** | A potential cause of an unwanted incident. |
| **Vulnerability** | A weakness that can be exploited by a threat. |
| **Residual Risk** | The risk remaining after controls are applied. |

## 4. Information Security Objectives

- Protect customer, transaction, and corporate data against unauthorised access, disclosure, alteration, and destruction.
- Meet all regulatory, contractual, and card-scheme security obligations (MAS TRM, PCI-DSS, partner-bank requirements).
- Maintain availability of critical services in line with documented RTO/RPO targets (Policy 09).
- Embed security-by-design across products and infrastructure.
- Continuously improve the ISMS based on risk assessments, audits, metrics, and incident learnings.

## 5. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| Board / Executive | Endorse the ISMS, allocate resources, approve risk appetite for security. |
| CISO | Owns the ISMS; chairs the Information Security Committee; reports posture to leadership. |
| Security Team | Operates and monitors security controls; runs assessments and the SoA. |
| IT / Engineering | Implements controls in systems they build and run. |
| Asset Owners | Classify assets and approve access. |
| Internal Audit | Independently assures the ISMS. |
| All Staff | Comply with security policies; report incidents and weaknesses. |

### 5.1 RACI — ISMS Activities

| Activity | CISO | Security Team | IT/Eng | Risk | Internal Audit |
|---|---|---|---|---|---|
| Maintain the ISMS & Statement of Applicability | A | R | C | I | I |
| Approve information security policy | A | C | I | I | C |
| Operate technical security controls | I | A | R | C | I |
| Conduct risk assessments | A | R | C | C | I |
| Internal ISMS audit | I | I | I | I | R |
| Report security posture to the Board | A | R | I | I | I |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 6. ISMS Governance & Operation

- The CISO owns the ISMS and reports security posture to executive leadership at least quarterly.
- An **Information Security Committee** meets at least quarterly to review risks, incidents, metrics, exceptions, and improvement actions.
- Security risk is managed under the Risk Management Policy (Policy 15); the resulting risk treatment plan drives the **Statement of Applicability**.
- The ISMS follows a **Plan-Do-Check-Act** cycle with a formal management review at least annually.

## 7. Core Control Domains (ISO 27001:2022 Annex A)

| Annex A Theme | Summary of Aspire Controls |
|---|---|
| A.5 Organisational | Policies, roles, segregation of duties, threat intelligence, supplier security, continuity, and legal/compliance controls. |
| A.6 People | Screening, terms of employment, awareness & training, disciplinary process, NDAs, remote-working rules (Policy 06, the relevant policy). |
| A.7 Physical | Secure areas, physical entry, equipment protection, clear desk/clear screen, secure disposal (Policy the relevant policy). |
| A.8 Technological | Access control, cryptography, secure configuration, logging & monitoring, malware defence, vulnerability management, network security, secure development (Policies 02, 10, 11, the relevant policy). |

## 8. Key Security Requirements (Procedures)

- **Risk-based control selection:** Controls are selected via a documented risk assessment and recorded in the SoA.
- **Least privilege & need-to-know:** Enforced per the Access Control Policy (Policy 02) and IAM Standard (see Policy Index).
- **Encryption:** Data is encrypted in transit and at rest per the Cryptography Policy (Policy 11).
- **Logging & monitoring:** Security-relevant events are logged, protected against tampering, and monitored via the SIEM (see Policy Index).
- **Secure SDLC:** Security is embedded across development per the SSDLC Standard (see Policy Index) and Change Management (Policy 10).
- **Vulnerability & patch management:** Systems are scanned and patched on a defined cadence with remediation SLAs (see Policy Index).
- **Asset management:** All assets are inventoried with an assigned owner and classification (Policy 03).
- **Incident management:** Handled under the Incident Response Policy (Policy 08).

## 9. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Establish and maintain an ISMS | ISO 27001 Cl. 4–10; SOC 2 CC1–CC9 |
| Leadership commitment & policy | ISO 27001 Cl. 5; SOC 2 CC1.0 |
| Risk assessment & treatment | ISO 27001 Cl. 6.1, 8.2, 8.3; SOC 2 CC3.0 |
| Statement of Applicability | ISO 27001 Cl. 6.1.3 d) |
| Performance evaluation & internal audit | ISO 27001 Cl. 9; SOC 2 CC4.0 |
| Continual improvement | ISO 27001 Cl. 10; SOC 2 CC4.2 |

## 10. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the GRC / exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 11. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CISO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| % Annex A controls implemented per SoA | ≥ 95% | Quarterly | CISO |
| Critical vulnerabilities open past SLA | 0 | Weekly | Security |
| Security incidents (SEV1/SEV2) | Trend ↓ | Monthly | CISO |
| % staff completing security awareness training | ≥ 98% | Quarterly | Security |
| Overdue ISMS corrective actions | 0 | Monthly | CISO |

## 12. Related Documents

- Access Control Policy (02)
- Data Classification & Handling (03)
- Cryptography & Key Management (11)
- Incident Response (08)
- Change Management (10)
- Network & Endpoint Security Standard (Policy 28)
- Logging, Monitoring & SIEM Standard (Policy 29)
- Vulnerability & Patch Management Standard (see Policy Index)
- Statement of Applicability; ISMS Scope Document

## 13. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
