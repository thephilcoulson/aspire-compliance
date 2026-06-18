# 10 — Change Management Policy

| | |
|---|---|
| **Policy Owner** | [CTO / Head of Engineering] |
| **Approved By** | [Executive] |
| **Version** | 1.0 (template) |
| **Effective Date** | [DATE] |
| **Review Cadence** | Annual |
| **Classification** | Internal |
| **Aligned Standard** | SOC 2 (Change Management); ISO/IEC 27001:2022 (A.8.32) |

---

## 1. Purpose

To ensure changes to production systems, applications, and infrastructure are made in a controlled, secure, and auditable manner, minimising risk to availability, integrity, and security.

## 2. Scope

All changes to production systems, code, configurations, and infrastructure, including emergency changes.

## 3. Change Principles

- **Authorised:** Every change is reviewed and approved before deployment.
- **Tested:** Changes are tested prior to production release.
- **Traceable:** Changes are tracked from request through deployment.
- **Segregation of duties:** Developers cannot unilaterally approve and deploy their own changes to production where feasible.

## 4. Change Categories

| Type | Definition | Approval |
|------|-----------|----------|
| Standard | Pre-approved, low-risk, repeatable | Pre-authorised |
| Normal | Requires review/testing | Change approver / CAB |
| Emergency | Urgent fix to restore service or patch critical vulnerability | Expedited approval + retrospective review |

## 5. Change Process

1. **Request** — documented in the change/ticketing system with rationale and rollback plan.
2. **Review & Approve** — peer review (code review/PR) and approval by an authorised approver.
3. **Test** — automated and/or manual testing in non-production.
4. **Deploy** — via controlled CI/CD pipeline; production access restricted.
5. **Verify** — post-deployment validation.
6. **Document** — record outcome; link to the change record.

## 6. Secure Development

- Security requirements are integrated into the SDLC.
- Code is peer-reviewed; secrets are not committed to source control.
- Automated security testing (SAST/DAST/dependency scanning) is performed in the pipeline.
- Separate development, staging, and production environments.

## 7. Emergency Changes

- May bypass standard lead times but require approval (verbal/expedited) and full retrospective documentation and review.

## 8. Rollback

- Every change includes a rollback or recovery plan.

## 9. Enforcement & Review

Unauthorised changes are investigated and may result in disciplinary action. Reviewed at least annually.
