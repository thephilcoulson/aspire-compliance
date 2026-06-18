# 02 — Access Control Policy

| | |
|---|---|
| **Policy Owner** | [CISO / Head of IT] |
| **Approved By** | [Executive] |
| **Version** | 1.0 (template) |
| **Effective Date** | [DATE] |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022 (A.5.15–A.5.18, A.8.2–A.8.5); SOC 2 |

---

## 1. Purpose

To ensure that access to Aspire's systems, applications, and data is granted, managed, and revoked based on the principles of least privilege and need-to-know.

## 2. Scope

All systems, applications, networks, and data, and all users (employees, contractors, service accounts, and third parties).

## 3. Principles

- **Least privilege:** Users receive the minimum access required for their role.
- **Need-to-know:** Access to sensitive data is restricted to those with a legitimate business need.
- **Segregation of duties:** Conflicting responsibilities (e.g. requesting and approving access) are separated.
- **Accountability:** Every action is attributable to a unique identity.

## 4. User Lifecycle Management

| Stage | Requirement |
|-------|-------------|
| Provisioning | Access granted via documented request and approval; role-based where possible. |
| Modification | Changes follow the same request/approval flow; reviewed on role change. |
| Deprovisioning | Access revoked within [4 hours / same business day] of termination. |
| Review | Access rights recertified at least [quarterly] for privileged and [semi-annually] for standard access. |

## 5. Authentication

- **Unique IDs:** Shared accounts are prohibited except where technically unavoidable and compensating controls exist.
- **Multi-Factor Authentication (MFA):** Required for all remote access, administrative access, and access to systems holding sensitive or cardholder data.
- **Passwords:** Must meet complexity and length standards; stored only as salted hashes; never transmitted in clear text.
- **Privileged access:** Managed via a Privileged Access Management (PAM) solution with session logging and just-in-time elevation where feasible.

## 6. Authorization

- Access is role-based (RBAC) and mapped to documented role definitions.
- Privileged/administrative access is restricted, logged, and reviewed.

## 7. Service & Machine Accounts

- Inventoried, owned, with credentials rotated and stored in a secrets manager.
- Non-interactive; no human use of service-account credentials.

## 8. Remote & Network Access

- All remote access via encrypted channels (VPN/zero-trust) with MFA.
- Network segmentation isolates sensitive environments (e.g. cardholder data environment).

## 9. Monitoring

- Access events are logged and monitored for anomalies.
- Failed authentication thresholds trigger account lockout and alerting.

## 10. Enforcement & Review

Violations may result in access revocation and disciplinary action. Reviewed at least annually.
