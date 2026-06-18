# 14 — PCI-DSS Cardholder Data Security Policy

| | |
|---|---|
| **Document ID** | POL-14 |
| **Policy Owner** | CISO |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal — Restricted |
| **Aligned Standard** | PCI-DSS v4.0 |

---

## 1. Purpose

To protect cardholder data (CHD) and sensitive authentication data (SAD) in accordance with the Payment Card Industry Data Security Standard (PCI-DSS) v4.0, wherever Aspire stores, processes, or transmits such data in connection with its card products.

## 2. Scope

The Cardholder Data Environment (CDE) — all people, processes, system components, and networks that store, process, or transmit CHD/SAD — and connected/security-impacting systems.

> **Scope minimisation:** Aspire shall minimise the CDE wherever possible (tokenisation, PCI-DSS-compliant processors, outsourcing card handling) to reduce scope and risk. CDE scope and card data flows are documented and validated at least annually.

## 3. Definitions & Glossary

| Term | Definition |
|------|------------|
| **CHD** | Cardholder Data — PAN, cardholder name, expiry, service code. |
| **SAD** | Sensitive Authentication Data — full track, CAV2/CVC2/CVV2/CID, PIN/PIN block. |
| **PAN** | Primary Account Number. |
| **CDE** | Cardholder Data Environment. |
| **Tokenisation** | Replacing PAN with a non-sensitive token. |
| **SAQ / ROC / AOC** | Self-Assessment Questionnaire / Report on Compliance / Attestation of Compliance. |
| **ASV** | Approved Scanning Vendor (external vulnerability scans). |
| **QSA** | Qualified Security Assessor. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| CISO | Owns the PCI-DSS program and CDE security. |
| Security Engineering | Implements and operates CDE controls. |
| Compliance | Manages SAQ/ROC, attestation, and evidence. |
| Vendor Risk | Tracks service-provider AOCs and responsibility matrices. |
| Acquirer / QSA | External validation and reporting. |

### 4.1 RACI — PCI-DSS Program

| Activity | CISO | Security Eng | Compliance | Acquirer/QSA |
|---|---|---|---|---|
| Maintain CDE scope & data-flow diagrams | A | R | C | I |
| Operate CDE security controls | A | R | C | I |
| Manage SAQ/ROC & attestation | A | C | R | I |
| Manage service-provider AOCs | C | R | A | I |
| Respond to card-data incidents | A | R | C | C |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. The 12 PCI-DSS Requirements (Control Summary)

1. **Install and maintain network security controls** — firewalls/segmentation isolate the CDE.
2. **Apply secure configurations** — no vendor defaults; hardened baselines.
3. **Protect stored account data** — minimise storage; never store SAD post-authorisation; render PAN unreadable (truncation, tokenisation, strong encryption per Policy 11).
4. **Protect cardholder data with strong cryptography during transmission** over open/public networks.
5. **Protect against malware** — anti-malware on applicable systems, kept current.
6. **Develop and maintain secure systems and software** — patching, secure SDLC, vulnerability remediation (Policy 10; SSDLC the relevant policy).
7. **Restrict access by business need-to-know** — least privilege (Policy 02).
8. **Identify users and authenticate access** — unique IDs, MFA for CDE access.
9. **Restrict physical access** to CHD and CDE systems/media (Policy the relevant policy).
10. **Log and monitor all access** to network resources and CHD; retain logs (≥12 months; 3 months readily available).
11. **Test security of systems and networks regularly** — internal/external (ASV) scans, penetration tests, file-integrity monitoring.
12. **Support information security with organisational policies and programs**, including personnel responsibilities and a targeted risk analysis (TRA) per v4.0.

## 6. Data Retention & Storage

- Store the minimum CHD necessary, only for as long as required.
- **Never store** SAD after authorisation (full track, CVV/CVV2, PIN/PIN block).
- Mask PAN when displayed (at most first six/last four) per business need.

## 7. Key Management

Cryptographic keys protecting CHD are managed per the Cryptography & Key Management Policy (11), including dual control and split knowledge.

## 8. Service Providers

Maintain a list of PCI-DSS-relevant service providers, their compliance status (AOC), and documented responsibility matrices (who covers which requirements) (Policy 07; Outsourcing the relevant policy).

## 9. Incident Response

Card-data incidents follow the Incident Response Policy (08) and card-scheme/acquirer breach procedures.

## 10. Compliance Validation

Complete the applicable SAQ or ROC and attestation per Aspire's merchant/service-provider level, at least annually, plus the v4.0 customised-approach/TRA documentation where used.

## 11. Control Objectives & Standards Mapping

| Control Objective | Mapped PCI-DSS v4.0 Requirement |
|---|---|
| Network security controls | Req. 1 |
| Secure configurations | Req. 2 |
| Protect stored account data | Req. 3 |
| Protect data in transit | Req. 4 |
| Vulnerability & secure software | Req. 5, 6, 11 |
| Access control & authentication | Req. 7, 8, 9 |
| Logging & monitoring | Req. 10 |
| Policy & program | Req. 12 |

## 12. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the GRC / exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 13. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CISO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| ASV scans passing | 100% | Quarterly | Security Eng |
| Critical CDE vulnerabilities open past SLA | 0 | Weekly | Security Eng |
| Service-provider AOCs current | 100% | Quarterly | Vendor Risk |
| Annual attestation completed on time | Yes | Annual | Compliance |

## 14. Related Documents

- Cryptography & Key Management (11)
- Access Control Policy (02)
- Change Management (10)
- Incident Response (08)
- Network & Endpoint Security Standard (Policy 28)
- Logging, Monitoring & SIEM Standard (Policy 29)
- Vulnerability & Patch Management Standard (see Policy Index)
- Physical & Environmental Security (see Policy Index)
- CDE Scope & Data-Flow Diagrams

## 15. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Confirm all role assignments, dates, thresholds, and cross-references against Aspire's actual environment first. Do not present to an auditor, regulator, or customer as-is.
