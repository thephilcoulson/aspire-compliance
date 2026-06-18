# Aspire — Compliance Policy Framework

A structured, industry-aligned compliance policy set for **Aspire** (aspireapp.com), the Southeast Asian business finance / all-in-one finance operating system for growing businesses.

> ⚠️ **IMPORTANT — READ FIRST**
> These documents are **AI-generated templates** intended as a *starting framework*, not certification-ready or legally binding policies. Every policy must be:
> 1. Reviewed and adapted by Aspire's legal, risk, and compliance functions
> 2. Mapped to the actual systems, processes, and regulatory licences Aspire holds in each jurisdiction
> 3. Formally approved by an accountable owner before being relied upon
>
> Do **not** present these to an auditor, regulator, or customer as-is.

---

## Scope

This framework covers a fintech operating across Southeast Asia (Singapore, and expansion markets) offering business accounts, payments, cards, expense management, and credit products. It is structured around the following standards and regimes:

| Domain | Standard / Regime |
|--------|-------------------|
| Information Security Management | ISO/IEC 27001:2022 |
| Service Organisation Controls | SOC 2 (Trust Services Criteria) |
| Cardholder Data | PCI-DSS v4.0 |
| Anti-Money Laundering / CFT | FATF, MAS Notices/Guidelines (PSN01/PSN02), AMLA |
| Customer Due Diligence | KYC / KYB |
| Data Privacy | Singapore PDPA, EU GDPR (where applicable) |
| Business Continuity | ISO 22301 (aligned) |

---

## Policy Index

| # | Policy | Primary Standard |
|---|--------|------------------|
| 00 | [Compliance Program Overview & Governance](policies/00-compliance-program-overview.md) | Cross-cutting |
| 01 | [Information Security Policy](policies/01-information-security-policy.md) | ISO 27001 |
| 02 | [Access Control Policy](policies/02-access-control-policy.md) | ISO 27001 / SOC 2 |
| 03 | [Data Classification & Handling Policy](policies/03-data-classification-handling.md) | ISO 27001 |
| 04 | [Data Privacy & Protection Policy](policies/04-data-privacy-protection.md) | PDPA / GDPR |
| 05 | [Acceptable Use Policy](policies/05-acceptable-use-policy.md) | ISO 27001 |
| 06 | [Human Resources Security Policy](policies/06-hr-security-policy.md) | ISO 27001 |
| 07 | [Vendor & Third-Party Risk Management Policy](policies/07-vendor-third-party-risk.md) | SOC 2 / ISO 27001 |
| 08 | [Incident Response & Breach Management Policy](policies/08-incident-response-policy.md) | ISO 27001 / SOC 2 |
| 09 | [Business Continuity & Disaster Recovery Policy](policies/09-business-continuity-dr.md) | ISO 22301 |
| 10 | [Change Management Policy](policies/10-change-management-policy.md) | SOC 2 |
| 11 | [Cryptography & Key Management Policy](policies/11-cryptography-key-management.md) | ISO 27001 / PCI-DSS |
| 12 | [Anti-Money Laundering & CFT Policy](policies/12-aml-cft-policy.md) | MAS / FATF |
| 13 | [Know Your Customer (KYC/KYB) Policy](policies/13-kyc-kyb-policy.md) | MAS / FATF |
| 14 | [PCI-DSS Cardholder Data Security Policy](policies/14-pci-dss-policy.md) | PCI-DSS v4.0 |
| 15 | [Risk Management Policy](policies/15-risk-management-policy.md) | ISO 27001 / Enterprise |
| 16 | [Code of Conduct & Ethics Policy](policies/16-code-of-conduct.md) | Governance |

---

## How to Use This Repository

1. **Assign owners** — each policy needs a named accountable owner (the *Document Control* table at the top of each file).
2. **Adapt, don't adopt** — replace bracketed `[PLACEHOLDERS]` and tailor controls to Aspire's real environment.
3. **Establish a review cadence** — annual review minimum; sooner on material change.
4. **Version control** — use this repo's git history as the policy change log. Approve changes via pull request.
5. **Map to evidence** — link each control to operational evidence (logs, tickets, configs) for audit readiness.

---

## Document Conventions

- `[PLACEHOLDER]` — must be completed before the policy is operational.
- "**shall**" — a mandatory control.
- "**should**" — a recommended control; deviations require documented risk acceptance.

---

_Generated as a compliance starting framework. Last generated: 2026-06-18._
