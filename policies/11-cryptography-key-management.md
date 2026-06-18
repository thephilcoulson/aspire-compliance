# 11 — Cryptography & Key Management Policy

| | |
|---|---|
| **Document ID** | POL-11 |
| **Policy Owner** | CISO |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022 (A.8.24); PCI-DSS v4.0 (Req. 3 & 4); MAS TRM |

---

## 1. Purpose

To ensure cryptography is used effectively to protect the confidentiality, integrity, and authenticity of information, and that cryptographic keys are managed securely throughout their lifecycle — protecting customer data, cardholder data, credentials, and the integrity of financial transactions.

## 2. Scope

All systems and data requiring cryptographic protection, and all cryptographic keys, secrets, and certificates managed by or on behalf of Aspire.

## 3. Definitions & Glossary

| Term | Definition |
|------|------------|
| **Symmetric / Asymmetric** | Cryptography using shared / public-private key pairs respectively. |
| **KMS** | Key Management Service. |
| **HSM** | Hardware Security Module. |
| **KEK / DEK** | Key-Encrypting Key / Data-Encrypting Key (envelope encryption). |
| **Dual control / split knowledge** | No single person can use/reconstruct a sensitive key alone. |
| **Key rotation** | Replacing a key with a new one on a schedule or trigger. |
| **PKI** | Public Key Infrastructure. |

## 4. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| CISO | Owns cryptographic standards and key-management governance. |
| Security Engineering | Operates KMS/HSM; performs rotation and revocation. |
| Platform / IT | Implements encryption in systems they run. |
| Key Custodians | Hold split-knowledge components for the most sensitive keys (e.g. CHD keys). |
| Risk | Reviews and approves cryptographic exceptions. |

### 4.1 RACI — Key Lifecycle

| Activity | CISO | Security Eng | Platform/IT | Risk |
|---|---|---|---|---|
| Define cryptographic standards | A | R | C | I |
| Operate KMS/HSM | A | R | I | I |
| Rotate / revoke keys | A | R | I | I |
| Manage certificates | C | R | A | I |
| Approve algorithm exceptions | A | C | I | C |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 5. Encryption Standards

- **In transit:** TLS 1.2+ (prefer TLS 1.3) for all data over untrusted networks; weak protocols/ciphers (SSL, TLS 1.0/1.1) disabled.
- **At rest:** AES-256 (or equivalent) for Restricted and Confidential data.
- **Hashing:** Strong, salted algorithms (Argon2/bcrypt/scrypt) for passwords; deprecated algorithms (MD5, SHA-1 for security purposes) prohibited.
- Only vetted, standard cryptographic libraries are used; no custom/home-grown cryptography.
- A cryptographic inventory (algorithms, key sizes, locations) is maintained to support crypto-agility and post-quantum readiness planning.

## 6. Key Management Lifecycle (Procedure)

| Stage | Requirement |
|---|---|
| Generation | Generated using approved methods and sufficient entropy (HSM/KMS-backed). |
| Storage | Stored in an HSM or managed KMS; never hard-coded or stored in plaintext; secrets in a secrets manager. |
| Distribution | Distributed via secure channels with access controls. |
| Rotation | Rotated on a defined schedule and upon suspected compromise. |
| Revocation | Revoked promptly when compromised or no longer needed. |
| Destruction | Securely destroyed/zeroised at end of life with records retained. |

## 7. Access to Keys

Access to cryptographic keys is restricted to authorised personnel on need-to-know, with **dual control and split knowledge** for the most sensitive keys (e.g. cardholder-data encryption keys per PCI-DSS).

## 8. Certificate & PKI Management

TLS and code-signing certificates are inventoried, monitored for expiry, and renewed before expiry; private keys are protected and never shared; automated certificate management is preferred.

## 9. PCI-DSS Specifics

Where cardholder data is encrypted, key-management procedures meet PCI-DSS Requirement 3, including documented key-custodian responsibilities, key-encrypting keys, and prevention of unauthorised key substitution.

## 10. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Use of cryptography | ISO 27001 A.8.24; SOC 2 CC6.1 |
| Protection of stored account data | PCI-DSS Req. 3 |
| Protection of data in transit | PCI-DSS Req. 4; ISO 27001 A.8.24 |
| Key management | PCI-DSS Req. 3.6–3.7; ISO 27001 A.8.24 |
| Secrets management | ISO 27001 A.8.24, A.5.17 |

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
| % Restricted data encrypted at rest | 100% | Quarterly | CISO |
| Certificates renewed before expiry | 100% | Monthly | Security Eng |
| Keys rotated within policy schedule | 100% | Quarterly | Security Eng |
| Hard-coded secrets detected in code | 0 | Monthly | Security |

## 13. Related Documents

- Information Security Policy (01)
- Data Classification & Handling (03)
- Access Control Policy (02)
- PCI-DSS Policy (14)
- Secure Software Development Lifecycle Standard (see Policy Index)
- Cryptographic Inventory

## 14. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
