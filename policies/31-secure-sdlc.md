# 31 — Secure Software Development Lifecycle (SSDLC) Standard

| | |
|---|---|
| **Document ID** | POL-31 |
| **Policy Owner** | Chief Technology Officer / CISO |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard / Regime** | ISO/IEC 27001:2022 (A.8.25–A.8.31); PCI-DSS Req. 6; OWASP ASVS/SAMM; SOC 2 |

---

## 1. Purpose

To embed security throughout the software development lifecycle so that Aspire's applications are designed, built, tested, and deployed securely, protecting customer data and financial transactions from common and emerging software risks.

## 2. Scope

All in-house and contracted software development, including services, APIs, mobile/web apps, and infrastructure-as-code.

## 3. Definitions & Glossary

| Term | Definition |
|---|---|
| SSDLC | Security integrated across the development lifecycle. |
| Threat Modelling | Structured analysis of design-level threats. |
| SAST / DAST | Static / Dynamic Application Security Testing. |
| SCA | Software Composition Analysis. |
| Secrets Scanning | Detecting credentials committed to code. |
| Security Champion | An engineer embedded with security responsibility. |
| OWASP | Open Worldwide Application Security Project. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|---|---|
| CTO / CISO | Co-own the SSDLC standard and security gates. |
| Engineering Teams | Build securely; remediate findings. |
| Application Security | Defines requirements, tooling, and reviews. |
| Security Champions | Drive secure practices within squads. |

### 4.1 RACI

| Activity | CTO/CISO | Eng Teams | AppSec | Champions |
|---|---|---|---|---|
| Define security requirements & gates | A | C | R | C |
| Threat model significant features | C | R | R | C |
| Run SAST/DAST/SCA in pipeline | A | R | R | I |
| Remediate security findings | C | R | C | R |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Secure Design & Threat Modelling

Security requirements are defined early; significant features and architectural changes undergo threat modelling. Designs apply secure-by-default principles: least privilege, input validation, output encoding, secure session management, and defence in depth, aligned to OWASP ASVS.

## 6. Secure Coding & Standards

Engineers follow secure-coding standards addressing the OWASP Top 10 and API security risks. Code is peer-reviewed; no secrets are committed (secret scanning enforced); dependencies are vetted and kept current (SCA).

## 7. Security Testing in the Pipeline

CI/CD enforces automated security gates: SAST, DAST, SCA, secrets scanning, and IaC scanning. Builds failing critical security gates do not proceed to production. Results integrate with vulnerability management (Policy the relevant policy).

## 8. Environments & Test Data

Development, staging, and production are separated (Policy 10). Production data is not used in lower environments unless masked/tokenised; cardholder data is never used in test environments (Policy 14).

## 9. Release & Post-Release

Changes deploy via controlled pipelines (Policy 10) with security sign-off for significant releases; post-release monitoring (Policy the relevant policy) detects issues; vulnerabilities found in production follow remediation SLAs (Policy the relevant policy).

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Secure development lifecycle | ISO 27001 A.8.25; PCI-DSS Req. 6.2 |
| Secure coding & application security | ISO 27001 A.8.28; OWASP ASVS |
| Security testing | ISO 27001 A.8.29; PCI-DSS Req. 6.3, 11.3 |
| Separation & protection of environments | ISO 27001 A.8.31; PCI-DSS Req. 6.5 |
| Test data protection | ISO 27001 A.8.33; PCI-DSS Req. 6.5 |

## 11. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the the GRC exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 12. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CTO and CISO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| Builds passing security gates | 100% | Per release | AppSec |
| Critical app vulns at release | 0 | Per release | AppSec |
| Threat models for significant features | 100% | Quarterly | AppSec |
| Secrets detected in code (unremediated) | 0 | Monthly | AppSec |

## 13. Related Documents

- Change Management (10)
- Vulnerability & Patch Management Standard (30)
- Cryptography & Key Management (11)
- Logging, Monitoring & SIEM Standard (29)
- PCI-DSS Policy (14)
- Secure Coding Standards

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
