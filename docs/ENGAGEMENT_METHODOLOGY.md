# Engagement Methodology

[← Back to main page](../README.md)

## Core Principle

**HARDEN → TEST → VALIDATE → REMEDIATE → RE-TEST → MAINTAIN**

Penetration testing is a component of the security lifecycle. Its value depends on validating whether weaknesses are real, fixing what matters and verifying the resulting security state.

## Standard Engagement Flow (Company Profile)

```text
Infrastructure / Software Installation
    → Penetration Test
    → Identify Vulnerabilities
    → Remediation
    → Final Penetration Test to Verify
    → Reporting
```

The stages below add operational preparation and safeguards necessary to conduct that flow responsibly.

## Stage 0 — Scope and Rules of Engagement

Identify system owners and authorized decision-makers. Confirm target inventory, testing location, environment, time windows, credentials, service dependencies, regulatory constraints, prohibitions, emergency contacts and testing stop conditions. Document expected deliverables and re-test windows. **No technical testing before written authorization.**

## Stage 1 — Understand the Environment

For whitebox and graybox work, review the approved architecture, functional expectations and available documentation. For blackbox work, limit initial assumptions and examine the authorized external surface. Record what has been provided versus what has actually been validated.

## Stage 2 — Assess the Approved Scope

Evaluate relevant services, trust boundaries, application behavior, authentication and business logic using proportionate methods. Account for availability, rate limits and production risk. Preserve traceability to specific scope items and observation times.

## Stage 3 — Validate Material Findings

Determine whether important findings are reproducible, relevant and actionable. Distinguish confirmed exploitation from potentially risky configurations, third-party scanner indications or findings requiring additional permissions. Avoid unnecessary data extraction or persistent changes.

## Stage 4 — Prioritize and Recommend Remediation

Document affected components, preconditions, observed behavior, likelihood and business effect, along with practical corrective guidance. Collaborate with the client on feasible priorities and operational impact. Urgent material findings may be escalated immediately using the agreed communication procedure.

## Stage 5 — Re-Test Corrected Weaknesses

Re-test findings once changes are deployed. Test not only that the observed condition is gone, but where appropriate that the defensive control now behaves correctly. Where a full re-test is impossible, clearly state limitations.

## Stage 6 — Final Report and Handover

Deliver agreed executive and technical records through a protected channel. Capture closed and open findings, testing constraints, scope exclusions, residual risk and next actions. Recommend periodic review according to changes in exposed services and threat conditions.

## Testing Styles

- **Whitebox:** extensive authorized knowledge for deeper review of internal implementation and configuration.
- **Graybox:** limited knowledge/privileges for partially trusted user and administrative boundary validation.
- **Blackbox:** little or no internal knowledge, focused on externally observable exposures and authorized attack-path validation.

The selected style does not automatically authorize destructive activity, unrestricted exploitation or access to third-party services.

## Evidence Principles

Evidence should be proportionate, reproducible, time-bound and minimal. Distinguish **observation**, **inference**, **assessor recommendation** and **verified correction**. Preserve client confidentiality, and do not place confidential evidence in a public GitHub repository.
