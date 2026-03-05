# OctoAcme — Project Planning

## Purpose
Turn an approved initiative into an actionable plan and backlog for delivery.

## Objectives
- Break work into shippable increments
- Identify dependencies and risks
- Align timelines, releases, and responsibilities

## Key Roles in Planning
The following roles are actively involved in planning. See [Roles & Personas](./octoacme-roles-and-personas.md) for full descriptions and [Responsibility Matrix — Phase 2](./octoacme-responsibility-matrix.md#phase-2-planning) for RACI assignments.

- **Project Manager** — Facilitates kickoff, maintains project plan and risk register, aligns timelines with Release Manager.
- **Product Manager** — Owns backlog prioritization and acceptance criteria.
- **Business Analyst** — Elicits requirements, writes user stories, and facilitates stakeholder input sessions.
- **Scrum Master** — Plans sprint capacity, advises on backlog sizing, and sets up sprint ceremonies.
- **UX Designer** — Provides design specifications and prototypes before development begins; see the [Handoff & Communication Checklist](./octoacme-handoff-checklist.md#1-requirements--ux-handoff-planning--execution) for UX handoff gates.
- **DevOps Engineer** — Confirms infrastructure and pipeline readiness for the planned increment; see the [Handoff & Communication Checklist](./octoacme-handoff-checklist.md#4-devops-dependencies-planning--execution) for DevOps dependency items.
- **Security Lead** — Reviews threat model for features involving sensitive data or new attack surfaces.

## Activities
1. Kickoff meeting with stakeholders and delivery team
2. Create prioritized backlog with acceptance criteria (Product Manager + Business Analyst)
3. Estimate scope (T-shirt sizing or story points)
4. Define Definition of Done (DoD)
5. Identify dependencies and integration points
6. Create release plan and milestone map (Project Manager + Release Manager)
7. Complete requirements and UX handoff gates before development starts

## Backlog Item Template
- Title:
- Description:
- Acceptance criteria:
- Priority:
- Estimate:
- Owner:
- Related docs/links:

## Sprint / Iteration Planning
- Timebox planning to agreed sprint length
- Pull items that meet DoD and have clear acceptance criteria
- Scrum Master confirms team capacity and flags impediments
- Ensure UX designs and requirements are ready before pulling items into sprint

## Risk & Dependency Management
- Capture in Risk Register:
  - ID, Description, Impact, Probability, Owner, Mitigation
- Mark cross-team dependencies in the project board and escalate during weekly syncs
- Security Lead contributes security-specific risks; see [Risk Management & Communication](./octoacme-risks-and-communication.md)

## Planning Checklist
- [ ] Project kickoff held
- [ ] Backlog prioritized and estimated
- [ ] Release timeline and milestones agreed (Project Manager + Release Manager)
- [ ] Definition of Done documented
- [ ] Initial test plan / QA approach drafted
- [ ] UX designs handed off for sprint items (see [Handoff & Communication Checklist §1](./octoacme-handoff-checklist.md#1-requirements--ux-handoff-planning--execution))
- [ ] DevOps infrastructure dependencies confirmed (see [Handoff & Communication Checklist §4](./octoacme-handoff-checklist.md#4-devops-dependencies-planning--execution))
- [ ] Threat model reviewed with Security Lead for sensitive features
