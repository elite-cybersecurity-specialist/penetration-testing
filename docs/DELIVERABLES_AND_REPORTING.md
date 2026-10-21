# Customer Deliverables & Reporting

[← Back to main page](../README.md)

## What an Assessment Report Should Explain

Reports are designed to support both business decisions and technical remediation. Actual components, disclosure levels and formats depend on the contractual scope.

### Executive Summary

State what was assessed, why it mattered, high-priority exposure, important limitations and the most urgent corrective decisions. Avoid suggesting complete system security when assessment coverage was limited.

### Scope and Methodology

Identify authorization, assessment dates, models (whitebox/graybox/blackbox), tested asset inventory, credentials or roles in general terms, exclusions, operational limitations and the reference frameworks used.

### Technical Findings

Each confirmed finding should include: ID, descriptive title, affected asset or component, severity and context, observation and validation status, attacker prerequisites, business/technical impact, minimal relevant evidence, corrective recommendation, and review owner if agreed.

### Remediation Plan

Group corrective action by priority, dependencies and operational constraints. Distinguish actions ECS performed from actions recommended for the customer or their vendors.

### Re-Test Record

For each relevant finding, record the re-test date, assessed build/configuration, method summary, evidence and outcome: **resolved**, **partially resolved**, **open**, or **not re-tested**. Record any newly identified regression risks separately.

### Residual Risk and Handover

Summarize exclusions, findings still open, areas not tested, accepted risks and future testing priorities. Deliver technical evidence through the approved secure transfer method.

## Evidence and Privacy

No screenshots containing production secrets, internal IP inventories, client credentials, exposed sensitive data, victim information or exploit material are suitable for a public portfolio unless explicitly cleared through a rigorous disclosure process. This repository contains **templates**, not authentic client reports.

[Report structure template →](../templates/REPORT_STRUCTURE_TEMPLATE.md)  
[Re-test template →](../templates/RETEST_VERIFICATION_TEMPLATE.md)
