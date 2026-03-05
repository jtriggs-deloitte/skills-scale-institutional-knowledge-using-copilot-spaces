# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Key Roles in Risk & Communication
The following roles are actively involved in risk management. See [Roles & Personas](./octoacme-roles-and-personas.md) for full descriptions and [Responsibility Matrix](./octoacme-responsibility-matrix.md) for RACI assignments.

- **Project Manager** — Owns the Risk Register, facilitates risk reviews, and escalates to the appropriate level.
- **Security Lead** — Identifies and owns security-specific risks; leads incident response for security events; reports risk status to Project Manager and Product Manager.
- **Business Analyst** — Flags requirement-driven risks (scope ambiguity, conflicting stakeholder needs).
- **DevOps Engineer** — Reports infrastructure and deployment risks; contributes to incident post-mortems.
- **Release Manager** — Tracks release-related risks; coordinates rollback planning.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution (all roles contribute; Project Manager aggregates)
- Assess: estimate impact and likelihood (Project Manager + relevant owner, e.g., Security Lead for security risks)
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs. Refer to [Stakeholder subtypes in Roles & Personas](./octoacme-roles-and-personas.md#stakeholders) for tailoring communication by audience (Executive Sponsor, Business Owner, End Users, Compliance/Legal).
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level → Scrum Master → Project Manager → Product Lead → Executive Sponsor
- For security incidents, Security Lead leads response; notify Security Lead immediately and follow the security incident runbook; Project Manager coordinates stakeholder notifications
- For infrastructure/deployment incidents, DevOps Engineer and Release Manager lead triage; Project Manager escalates if business-impacting
- See [Handoff & Communication Checklist §2](./octoacme-handoff-checklist.md#2-security-review-checkpoint-execution--release) for security review gates before release
