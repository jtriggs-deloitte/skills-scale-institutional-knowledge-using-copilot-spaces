# OctoAcme — Handoff & Communication Checklist

This checklist is used during **planning and execution** to ensure clear handoffs between roles, reduce ambiguity, and confirm key dependencies are resolved before advancing through lifecycle gates. Reference the [Roles & Personas](./octoacme-roles-and-personas.md) document for role definitions and the [Responsibility Matrix](./octoacme-responsibility-matrix.md) for full RACI assignments.

---

## How to use this checklist

1. Copy the relevant section(s) into your sprint plan, release doc, or meeting notes.
2. Assign an owner to each item.
3. Check items off as they are confirmed complete.
4. Unresolved items must be escalated before proceeding to the next phase.

---

## 1. Requirements & UX Handoff (Planning → Execution)

Confirm before development begins on a new feature or initiative.

### Requirements Readiness (Business Analyst → Developer)
- [ ] User stories are written with clear acceptance criteria
- [ ] Edge cases and out-of-scope items are documented
- [ ] Stakeholder sign-off on requirements obtained (Business Analyst + Product Manager)
- [ ] Requirements are linked to backlog items in the project board

### UX Design Handoff (UX Designer → Developer)
- [ ] Wireframes and/or high-fidelity designs are finalized and linked in the ticket
- [ ] Annotated component specs (spacing, states, accessibility notes) are provided
- [ ] Design system components or reusable assets are identified
- [ ] UX Designer is available for implementation questions during sprint
- [ ] Prototype or walkthrough review completed with Developer before build starts

---

## 2. Security Review Checkpoint (Execution → Release)

Confirm before code is promoted to release candidate.

### Security Review (Developer + Security Lead)
- [ ] Threat model reviewed for new features handling sensitive data
- [ ] Static analysis / SAST scan completed with no critical or high open findings
- [ ] Dependency vulnerability scan completed (no critical unresolved CVEs)
- [ ] Secrets management reviewed (no hardcoded credentials)
- [ ] Security Lead has reviewed and approved changes (or granted exception with documented rationale)

---

## 3. Release Readiness (Execution → Release & Deployment)

Confirm before a release is scheduled for production.

### Technical Readiness (Developer + DevOps Engineer)
- [ ] All acceptance criteria met and PRs merged to release branch
- [ ] CI pipeline passing (build, test, lint, security scan)
- [ ] Environment parity confirmed by DevOps Engineer (staging matches production config)
- [ ] Smoke tests passing in staging environment
- [ ] Database migrations or configuration changes documented and rehearsed

### Release Coordination (Release Manager)
- [ ] Release schedule and deployment window confirmed with DevOps Engineer
- [ ] Rollback plan documented and rehearsed
- [ ] Release notes drafted and reviewed by Product Manager
- [ ] Security sign-off received from Security Lead
- [ ] Stakeholder communication drafted and ready to send post-deploy
- [ ] On-call coverage confirmed for deployment window

### Go / No-Go Decision (Release Manager)
- [ ] All items above checked or exceptions documented
- [ ] Go/No-Go meeting held with Release Manager, Project Manager, Product Manager, and Security Lead
- [ ] Decision recorded in the project log

---

## 4. DevOps Dependencies (Planning → Execution)

Confirm before beginning work that requires infrastructure changes or new pipeline capabilities.

### Infrastructure & CI/CD (DevOps Engineer)
- [ ] Environment requirements (dev, staging, production) documented for the sprint
- [ ] Any new infrastructure resources provisioned or scheduled
- [ ] Pipeline changes (new stages, secrets, environment variables) reviewed and merged
- [ ] Monitoring and alerting configured for new services or critical paths
- [ ] DevOps Engineer has confirmed capacity for deployment support during the sprint

---

## 5. Sprint Ceremony Readiness (Scrum Master)

Confirm before each sprint begins.

- [ ] Backlog groomed and top items estimated by the team
- [ ] Sprint goal agreed upon by Scrum Master, Product Manager, and team
- [ ] Team capacity documented (leave, part-time, onboarding)
- [ ] Dependencies from previous sprint identified and resolved or accepted
- [ ] Impediment log reviewed and outstanding items escalated if needed

---

## 6. Stakeholder Communication (Project Manager)

Confirm at key milestones and release points.

- [ ] Stakeholder list is current and communication preferences are documented
- [ ] Executive Sponsor notified of upcoming major releases or scope changes
- [ ] Business Owner / Product Sponsor has confirmed feature acceptance
- [ ] End User representatives have completed UAT (if applicable)
- [ ] Compliance / Legal sign-off obtained for regulatory-sensitive deliverables
- [ ] Weekly status update sent with progress, risks, and decisions needed

---

## 7. Post-Release Handoff (Release → Retrospective)

Confirm immediately after a production deployment.

- [ ] Post-deploy verification completed and results documented
- [ ] Release announcement sent to stakeholders (Release Manager + Project Manager)
- [ ] Any incidents during deployment documented in the incident log
- [ ] Monitoring dashboards reviewed for anomalies (DevOps Engineer)
- [ ] Retrospective scheduled (Scrum Master)
- [ ] Action items from this release added to the backlog

---

> For escalation paths and risk communication, see [Risk Management & Communication](./octoacme-risks-and-communication.md).
> For the full deployment process, see [Release & Deployment Guide](./octoacme-release-and-deployment.md).
