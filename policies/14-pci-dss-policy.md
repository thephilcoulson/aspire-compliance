# 14 — PCI-DSS Cardholder Data Security Policy

| | |
|---|---|
| **Policy Owner** | [CISO] |
| **Approved By** | [Executive] |
| **Version** | 1.0 (template) |
| **Effective Date** | [DATE] |
| **Review Cadence** | Annual |
| **Classification** | Internal — Restricted |
| **Aligned Standard** | PCI-DSS v4.0 |

---

## 1. Purpose

To protect cardholder data (CHD) and sensitive authentication data (SAD) in accordance with the Payment Card Industry Data Security Standard (PCI-DSS) v4.0, where Aspire stores, processes, or transmits such data.

## 2. Scope

The Cardholder Data Environment (CDE) — all people, processes, systems, and networks that store, process, or transmit CHD/SAD, and connected systems.

> **Scope minimisation:** Aspire shall minimise the CDE wherever possible (e.g. tokenisation, use of PCI-DSS-compliant payment processors, and outsourcing card handling) to reduce scope and risk.

## 3. The 12 PCI-DSS Requirements (Control Summary)

1. **Install and maintain network security controls** — firewalls/segmentation isolate the CDE.
2. **Apply secure configurations** — no vendor defaults; hardened baselines.
3. **Protect stored account data** — minimise storage; never store SAD post-authorisation; render PAN unreadable (truncation, tokenisation, strong encryption per Policy 11).
4. **Protect data in transit** — strong cryptography over open/public networks.
5. **Protect against malware** — anti-malware on applicable systems, kept current.
6. **Develop and maintain secure systems** — patching, secure SDLC, vulnerability remediation (link Policy 10).
7. **Restrict access by business need-to-know** — least privilege (link Policy 02).
8. **Identify users and authenticate access** — unique IDs, MFA for CDE access.
9. **Restrict physical access** to CHD and CDE systems/media.
10. **Log and monitor all access** to network resources and CHD; retain logs (≥12 months, 3 months readily available).
11. **Test security regularly** — vulnerability scans (incl. ASV), penetration tests, file-integrity monitoring.
12. **Maintain an information security policy** and program, including personnel responsibilities.

## 4. Data Retention & Storage

- Store the minimum CHD necessary, only for as long as required.
- **Never store** sensitive authentication data (full track, CVV/CVV2, PIN/PIN block) after authorisation.
- Mask PAN when displayed (show at most first six/last four) per business need.

## 5. Key Management

- Cryptographic keys protecting CHD are managed per the Cryptography & Key Management Policy (Policy 11), including dual control and split knowledge.

## 6. Service Providers

- Maintain a list of PCI-DSS-relevant service providers, their compliance status (AOC), and documented responsibility matrices (who covers which requirements).

## 7. Incident Response

- Card-data incidents follow the Incident Response Policy (Policy 08) and card-scheme/acquirer breach procedures.

## 8. Compliance Validation

- Complete the applicable SAQ or Report on Compliance (ROC) and attestation per Aspire's merchant/service-provider level, at least annually.

## 9. Enforcement & Review

Violations may result in disciplinary action, fines, and loss of card-processing privileges. Reviewed at least annually.
