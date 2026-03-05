# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Key Roles in Execution
The following roles are actively involved during execution. See [Roles & Personas](./octoacme-roles-and-personas.md) for full descriptions and [Responsibility Matrix — Phase 3](./octoacme-responsibility-matrix.md#phase-3-execution--tracking) for RACI assignments.

- **Scrum Master** — Facilitates daily standups, removes blockers, and tracks sprint health.
- **Developer** — Implements features, participates in code reviews, and runs automated tests.
- **UX Designer** — Available for implementation questions and validates UI against designs during sprint reviews.
- **DevOps Engineer** — Maintains CI/CD pipelines and monitors system health; reports pipeline issues to Project Manager and Release Manager.
- **Security Lead** — Reviews code and PRs for security issues; escalates findings to Project Manager.

## Team Rhythm
- Daily standups (15 min, facilitated by Scrum Master) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks (Project Manager + Product Manager)
- Demo/Review at the end of each sprint or milestone (Scrum Master facilitates, Developers present)

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review (DevOps Engineer maintains CI)
  - Require at least one approval before merging (or team-defined policy)
  - Security Lead reviews PRs for features touching sensitive data or infrastructure

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI (configured and maintained by DevOps Engineer)
- Manual QA for feature acceptance when needed
- UX Designer validates UI implementation against design specs before sprint sign-off

## Reporting & Metrics
- Scrum Master tracks velocity and burndown; shares with Project Manager
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage) — DevOps Engineer owns monitoring setup

## Blocker Escalation
- Level 1: Team-level triage in daily standup (Scrum Master)
- Level 2: Project Manager escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues
- Security incidents: Follow the Security Lead's incident response protocol; see [Risk Management & Communication](./octoacme-risks-and-communication.md)

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests, lint, and security scanning (DevOps Engineer)
- [ ] Regular demos scheduled (Scrum Master)
- [ ] Risk register updated weekly (Project Manager + Security Lead)
- [ ] UX implementation validated by UX Designer at sprint review
- [ ] See [Handoff & Communication Checklist](./octoacme-handoff-checklist.md) for cross-role handoff gates
