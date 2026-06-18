# 11 — Cryptography & Key Management Policy

| | |
|---|---|
| **Policy Owner** | [CISO] |
| **Approved By** | [Executive] |
| **Version** | 1.0 (template) |
| **Effective Date** | [DATE] |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022 (A.8.24); PCI-DSS v4.0 (Req. 3 & 4) |

---

## 1. Purpose

To ensure cryptography is used effectively to protect the confidentiality, integrity, and authenticity of information, and that cryptographic keys are managed securely throughout their lifecycle.

## 2. Scope

All systems and data requiring cryptographic protection, and all cryptographic keys and certificates managed by Aspire.

## 3. Encryption Standards

- **In transit:** TLS 1.2+ (prefer TLS 1.3) for all data transmission over untrusted networks. Weak protocols/ciphers (SSL, TLS 1.0/1.1) are disabled.
- **At rest:** AES-256 (or equivalent industry-standard) for Restricted and Confidential data.
- **Hashing:** Use strong, salted algorithms (e.g. bcrypt/scrypt/Argon2) for passwords. Deprecated algorithms (MD5, SHA-1 for security) are prohibited.
- Only vetted, standard cryptographic libraries are used; no custom/home-grown cryptography.

## 4. Key Management Lifecycle

| Stage | Requirement |
|-------|-------------|
| Generation | Generated using approved methods and sufficient entropy. |
| Storage | Stored in a hardware security module (HSM) or managed KMS; never hard-coded or stored in plaintext. |
| Distribution | Distributed via secure channels with access controls. |
| Rotation | Rotated on a defined schedule and upon suspected compromise. |
| Revocation | Revoked promptly when compromised or no longer needed. |
| Destruction | Securely destroyed at end of life. |

## 5. Access to Keys

- Access to cryptographic keys is restricted to authorised personnel on a need-to-know basis with dual control / split knowledge for the most sensitive keys (e.g. cardholder data encryption keys per PCI-DSS).

## 6. Certificate Management

- TLS certificates are inventoried, monitored for expiry, and renewed before expiry.
- Private keys are protected and never shared.

## 7. PCI-DSS Specifics

- Where cardholder data is encrypted, key-management procedures meet PCI-DSS Requirement 3, including documented key custodian responsibilities and key-encrypting keys.

## 8. Enforcement & Review

Violations may result in disciplinary action. Reviewed at least annually and on cryptographic standard changes.
