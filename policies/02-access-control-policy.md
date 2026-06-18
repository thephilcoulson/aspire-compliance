# 2 — Access Control Policy

| | |
|---|---|
| **Document ID** | POL-02 |
| **Policy Owner** | CISO / Head of IT |
| **Approved By** | Executive |
| **Version** | 1.0 (template) |
| **Effective Date** | 1 January 2026 |
| **Last Reviewed** | 1 January 2026 |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022 (A.5.15–A.5.18, A.8.2–A.8.5); SOC 2; PCI-DSS Req. 7 & 8 |

---

## 1. Purpose

To ensure that access to Aspire's systems, applications, networks, and data is granted, managed, reviewed, and revoked on the principles of least privilege, need-to-know, and segregation of duties — thereby protecting customer funds, personal data, cardholder data, and the integrity of Aspire's financial platform.

## 2. Scope

All systems, applications, networks, datastores, and physical access points, and all identities (employees, contractors, service/machine accounts, API clients, and authorised third parties) across all environments (production, staging, development, corporate).

## 3. Definitions & Glossary

| Term | Definition |
|------|------------|
| **RBAC** | Role-Based Access Control — access granted via roles mapped to job functions. |
| **ABAC** | Attribute-Based Access Control — access decisions based on attributes/context. |
| **PAM** | Privileged Access Management — controls for elevated/administrative accounts. |
| **JIT** | Just-in-Time access — temporary elevation granted for a bounded time. |
| **SoD** | Segregation of Duties — splitting conflicting responsibilities. |
| **Recertification** | Periodic review confirming access is still appropriate. |
| **Service account** | A non-human identity used by an application or process. |

## 4. Principles

- **Least privilege:** Users and accounts receive only the minimum access required.
- **Need-to-know:** Access to sensitive data is restricted to a legitimate business need.
- **Segregation of duties:** Conflicting responsibilities (e.g. request vs. approve, develop vs. deploy to production) are separated.
- **Accountability:** Every action is attributable to a unique identity; shared accounts are prohibited save for documented, compensated exceptions.
- **Default deny:** Access is denied unless explicitly granted.

## 5. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| CISO / Head of IT | Owns the access control framework and PAM tooling. |
| IT / IAM Team | Executes provisioning, modification, deprovisioning, and recertification. |
| Line Managers | Request and approve access appropriate to a role; confirm at recertification. |
| System / Data Owners | Define role-to-entitlement mappings and approve sensitive access. |
| Security / Internal Audit | Monitor access events and audit entitlements. |

### 5.1 RACI — Access Lifecycle

| Activity | IT/IAM Team | CISO | Line Manager | Security/Audit |
|---|---|---|---|---|
| Approve access requests | I | A | R | C |
| Provision / deprovision access | R | A | I | I |
| Perform access recertification | R | A | C | I |
| Manage privileged access (PAM) | R | A | C | I |
| Investigate access violations | C | A | I | R |

> **RACI legend:** **R** = Responsible (does the work) · **A** = Accountable (ultimately answerable; one per row) · **C** = Consulted (two-way input) · **I** = Informed (kept up to date).

## 6. User Lifecycle Management (Procedures)

| Stage | Requirement |
|---|---|
| Joiner / Provisioning | Access granted via a documented request and manager + owner approval; role-based where possible; no standing privileged access by default. |
| Mover / Modification | On role change, entitlements are re-baselined to the new role; legacy access is removed (no privilege accumulation). |
| Leaver / Deprovisioning | All access revoked within 4 hours / same business day of termination; immediate for involuntary terminations. |
| Recertification | Privileged access recertified at least quarterly; standard access semi-annually; orphaned/unused accounts disabled. |

## 7. Authentication

- **Unique IDs:** Every user and service has a unique identifier. Shared/generic accounts are prohibited except where technically unavoidable and compensating controls (logging, restricted custody) exist and are approved.
- **Multi-Factor Authentication (MFA):** Required for all remote access, all administrative access, and all access to systems holding Restricted/Confidential or cardholder data. Phishing-resistant MFA (FIDO2/WebAuthn) is preferred for privileged users.
- **Passwords:** Meet length/complexity standards; stored only as salted hashes (Argon2/bcrypt/scrypt); never transmitted or stored in clear text; checked against breached-password lists.
- **Privileged access:** Managed via a PAM solution with credential vaulting, session recording, and just-in-time elevation where feasible.
- **API & machine authentication:** Token/key-based, short-lived where possible, stored in a secrets manager.

## 8. Authorization

- Access is role-based (RBAC), mapped to documented role definitions and an entitlement catalogue.
- Privileged/administrative access is restricted, logged, time-bound, and reviewed.
- High-risk SoD conflicts (e.g. payment initiation and approval) are defined in an SoD matrix and prevented or detected with compensating controls.

## 9. Service & Machine Accounts

- Inventoried, owned, classified, with credentials rotated on a defined schedule and stored in a secrets manager.
- Non-interactive; no human use of service-account credentials; scoped to least privilege.

## 10. Remote & Network Access

- All remote access via encrypted channels (VPN / zero-trust network access) with MFA.
- Network segmentation isolates sensitive environments (e.g. the cardholder data environment) per the Network Security Standard (see Policy Index).

## 11. Monitoring

- Access events (authentication, authorisation, privilege use) are logged to the SIEM and monitored for anomalies (see Policy Index).
- Failed-authentication thresholds trigger lockout and alerting; impossible-travel and privilege-escalation patterns are alerted.

## 12. Control Objectives & Standards Mapping

| Control Objective | Mapped Standard / Clause |
|---|---|
| Identity & access management | ISO 27001 A.5.15, A.5.16, A.5.18; SOC 2 CC6.1–CC6.3 |
| Privileged access management | ISO 27001 A.8.2; SOC 2 CC6.1; PCI-DSS Req. 7 |
| Authentication & MFA | ISO 27001 A.8.5; PCI-DSS Req. 8; MAS TRM |
| Access recertification | ISO 27001 A.5.18; SOC 2 CC6.3; PCI-DSS Req. 7.2 |
| Segregation of duties | ISO 27001 A.5.3; SOC 2 CC6.3 |

## 13. Exceptions & Waivers

Any deviation from this policy requires a formal, time-bound exception.

1. **Request:** The requester logs an exception in the GRC / exception register describing the control deviated from, the business justification, the compensating controls, and the requested expiry date.
2. **Risk assessment:** The relevant control owner and the Risk function assess the residual risk of the deviation.
3. **Approval authority:** Exceptions are approved by the Policy Owner for low/medium residual risk and by the CISO/CCO and, where material, the Audit & Risk Committee for high residual risk.
4. **Time limits:** Exceptions are granted for a maximum of 90 days and must be re-reviewed before renewal. No exception is open-ended.
5. **Tracking:** All approved exceptions are recorded in the exception register with an owner, expiry, and remediation plan, and are reported in periodic compliance reporting.
6. **Revocation:** Exceptions may be revoked at any time if the residual risk changes or the compensating controls fail.

## 14. Metrics & KPIs

The following indicators are tracked to measure the effectiveness of this policy and reported to the CISO and, where material, the Audit & Risk Committee.

| Metric / KPI | Target | Frequency | Owner |
|---|---|---|---|
| % deprovisioning completed within SLA | 100% | Monthly | IAM Team |
| Privileged accounts with JIT/PAM coverage | ≥ 95% | Quarterly | CISO |
| Access recertification completion | 100% | Quarterly | IAM Team |
| Orphaned/dormant accounts | 0 | Monthly | IAM Team |
| MFA coverage on in-scope systems | 100% | Monthly | Security |

## 15. Related Documents

- Identity & Access Management Standard (see Policy Index)
- Information Security Policy (01)
- Cryptography & Key Management (11)
- Network & Endpoint Security Standard (Policy 28)
- HR Security Policy (06)
- PCI-DSS Policy (14)
- SoD Matrix; Entitlement Catalogue

## 16. Revision History

| Version | Date | Author | Reviewer / Approver | Summary of Change |
|---|---|---|---|---|
| 0.1 (draft) | 15 November 2025 | Compliance Team | Chief Compliance Officer | Initial AI-generated draft. |
| 1.0 (template) | 1 January 2026 | Compliance Team | Board of Directors | Baseline template issued for tailoring. |
| 1.1 | 1 January 2027 | Compliance Team | Board of Directors | Periodic review and update |

---

> ⚠️ **AI-GENERATED TEMPLATE.** This document is a starting framework, not certification-ready or legally binding. It must be reviewed, tailored to Aspire's actual systems, licences, and jurisdictions, and formally approved by an accountable owner before operational use. Replace all `[PLACEHOLDER]` values. Do not present to an auditor, regulator, or customer as-is.
