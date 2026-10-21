# Scoping, Authorization and Rules of Engagement

[← Back to main page](../README.md)

This page describes the **pre-engagement process**, not a substitute for a signed contract or legal advice.

## Information To Establish Before Testing

| Area | Agreement required |
|---|---|
| Ownership and written authority | Who can authorize each asset, network, building, application and third-party service? |
| Asset inventory | Domains, IP ranges, cloud accounts, apps, APIs, wireless networks, devices or sites expressly in scope. |
| Exclusions | Third-party providers, personal accounts, production payment flows, healthcare/safety systems or other protected assets. |
| Testing access | Test credentials, roles, source access, permitted vantage points and approved equipment. |
| Availability requirements | Business-critical times, service limits, rate restrictions, backup/recovery readiness. |
| Sensitive information | Data categories, recording restrictions, test-data use, retention and secure evidence transfer. |
| Staff/physical exercises | Separate approval for phishing, social engineering or physical security scenarios. |
| Emergency processes | Primary contacts, escalation channels, stop-work authority and critical-finding notifications. |
| Reporting | Deliverables, handling classification, due dates, recipients and remediation/re-test terms. |

## Written Rules of Engagement

The signed RoE should define precisely:

1. Legal entities and named authorizers.
2. In-scope systems and exclusions (including infrastructure hosted by third parties).
3. Permitted techniques and required approvals for higher-risk actions.
4. Assessment time window and geography.
5. Production service protections, traffic limits and forbidden disruptive tests.
6. Approved test accounts, privilege ceilings and data types.
7. Evidence collection, encryption, retention and deletion rules.
8. Emergency contacts, escalation timing and stop-work conditions.
9. Remediation ownership, re-test scope and reporting recipients.
10. Signed acceptance before work begins, plus documented change control for later scope additions.

## Activities That Require Explicit, Separate Approval

Any destructive testing, sustained denial-of-service, deliberate system downtime, mass messaging, personnel deception, physical entry, malware simulation with persistence, credential spraying, sensitive-data extraction or third-party access must have clear consent, necessity, safeguards and agreed limitations. If authorization is absent, the activity is not performed.

## Customer Responsibilities

Customers should ensure legitimate authority over assets, identify business-critical systems, coordinate vendors as necessary, arrange backups/change control and identify incident-response personnel. The assessor should document uncertainties and stop when the authorization boundary becomes unclear.

## Scope-Change Control

Record newly discovered assets as **potentially relevant but out of scope** until a designated authorizer signs a scope amendment. Discovery does not grant testing permission.

[Scoping questionnaire template →](../templates/SCOPING_QUESTIONNAIRE.md)  
[Rules of Engagement template →](../templates/RULES_OF_ENGAGEMENT_TEMPLATE.md)
