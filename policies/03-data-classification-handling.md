# 03 — Data Classification & Handling Policy

| | |
|---|---|
| **Policy Owner** | [CISO / DPO] |
| **Approved By** | [Executive] |
| **Version** | 1.0 (template) |
| **Effective Date** | [DATE] |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | ISO/IEC 27001:2022 (A.5.12–A.5.13) |

---

## 1. Purpose

To ensure information is classified according to its sensitivity and handled with controls appropriate to its classification throughout its lifecycle.

## 2. Scope

All information assets, in any form (electronic, physical, verbal), owned or processed by Aspire.

## 3. Classification Levels

| Level | Definition | Examples |
|-------|-----------|----------|
| **Restricted** | Highest sensitivity; severe harm if disclosed. | Cardholder data, credentials, KYC documents, encryption keys, banking details. |
| **Confidential** | Sensitive business or personal data. | Customer PII, financial records, contracts, source code. |
| **Internal** | Internal-use information. | Internal docs, policies, project plans. |
| **Public** | Approved for public release. | Marketing materials, published terms. |

## 4. Handling Requirements

| Control | Restricted | Confidential | Internal | Public |
|---------|-----------|--------------|----------|--------|
| Encryption at rest | Required | Required | Recommended | Optional |
| Encryption in transit | Required | Required | Required | Optional |
| Access control | Strict need-to-know + MFA | Need-to-know | Authenticated staff | Open |
| External sharing | Prohibited without DPO/CISO approval | Approval + agreement | Limited | Permitted |
| Retention | Per legal/regulatory schedule | Per schedule | Per schedule | N/A |
| Disposal | Secure wipe / shred | Secure wipe / shred | Standard delete | N/A |

## 5. Labelling

- Restricted and Confidential assets should be labelled where technically feasible.
- Default classification for unlabelled internal data is **Internal**.

## 6. Storage & Transmission

- Restricted and Confidential data must reside only in approved systems and locations.
- Transmission outside Aspire requires encryption and, for personal data, a lawful basis and appropriate safeguards.

## 7. Retention & Disposal

- Data is retained only as long as legally or operationally required (see Privacy Policy 04).
- Disposal uses methods that render data unrecoverable.

## 8. Responsibilities

- **Data owners** assign and maintain classification.
- **All users** handle data per its classification.

## 9. Enforcement & Review

Violations may result in disciplinary action. Reviewed at least annually.
