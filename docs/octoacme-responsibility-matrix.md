# OctoAcme — Responsibility Matrix

This document provides a RACI-style responsibility matrix mapping core project lifecycle activities to the roles defined in [Roles & Personas](./octoacme-roles-and-personas.md).

**RACI Key:**
- **R** = Responsible (does the work)
- **A** = Accountable (owns the outcome; approves)
- **C** = Consulted (provides input before decisions)
- **I** = Informed (notified of outcomes)

---

## Phase 1: Initiation

| Activity | Project Mgr | Product Mgr | Business Analyst | Scrum Master | UX Designer | Developer | DevOps Engineer | Release Manager | Security Lead | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|
| Define business need & success metrics | C | A | R | I | C | I | I | I | C | C |
| Identify stakeholders & communication plan | A | C | R | I | I | I | I | I | I | C |
| Draft Project One-pager | R | C | C | I | I | I | I | I | I | A |
| Initial risk identification | R | C | C | I | I | C | C | I | R | I |
| Go/No-Go decision | C | C | C | I | I | I | I | I | I | A |

> See [Project Initiation Guide](./octoacme-project-initiation.md) for deliverables and the initiation checklist.

---

## Phase 2: Planning

| Activity | Project Mgr | Product Mgr | Business Analyst | Scrum Master | UX Designer | Developer | DevOps Engineer | Release Manager | Security Lead | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|
| Backlog creation & prioritization | C | A | R | C | C | C | I | I | I | C |
| Requirements elicitation & user stories | I | C | A/R | C | C | R | I | I | C | C |
| UX design & prototype review | I | C | C | I | A/R | C | I | I | I | C |
| Sprint capacity planning | C | I | I | A/R | I | R | I | I | I | I |
| Release plan & milestone map | A | C | C | C | I | C | C | R | I | I |
| Definition of Done documentation | C | C | C | A/R | C | R | C | C | C | I |
| Risk register setup | A | C | C | I | I | C | C | I | R | I |
| Infrastructure & environment planning | I | I | I | I | I | C | A/R | C | C | I |
| Security threat modeling | I | C | C | I | I | C | C | I | A/R | I |

> See [Project Planning](./octoacme-project-planning.md) and the [Handoff & Communication Checklist](./octoacme-handoff-checklist.md) for planning-phase checklists.

---

## Phase 3: Execution & Tracking

| Activity | Project Mgr | Product Mgr | Business Analyst | Scrum Master | UX Designer | Developer | DevOps Engineer | Release Manager | Security Lead | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|
| Daily standup facilitation | I | I | I | A/R | I | R | I | I | I | I |
| Feature development | I | C | C | I | C | A/R | C | I | C | I |
| UI implementation & UX validation | I | C | C | I | A | R | I | I | I | I |
| CI/CD pipeline maintenance | I | I | I | I | I | C | A/R | C | C | I |
| Code & security review | I | I | I | I | I | R | C | I | A/R | I |
| Blocker identification & escalation | A | C | I | R | I | R | R | I | C | I |
| Sprint review / demo | C | A | C | R | C | R | I | I | I | I |
| Progress & velocity reporting | R | I | I | C | I | I | I | I | I | I |
| Risk register updates | A | C | C | I | I | C | C | I | R | I |

> See [Execution & Tracking](./octoacme-execution-and-tracking.md) for team rhythms, PR workflows, and escalation levels.

---

## Phase 4: Release & Deployment

| Activity | Project Mgr | Product Mgr | Business Analyst | Scrum Master | UX Designer | Developer | DevOps Engineer | Release Manager | Security Lead | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|
| Release readiness review (go/no-go) | C | C | I | I | C | C | C | A/R | C | I |
| Security sign-off | I | I | I | I | I | I | C | C | A/R | I |
| Deployment execution | I | I | I | I | I | C | R | A | I | I |
| Smoke testing & post-deploy verification | I | I | I | I | I | R | C | A | I | I |
| Release notes drafting | I | C | C | I | I | C | I | A/R | C | I |
| Stakeholder release communication | R | C | I | I | I | I | I | C | I | I |
| Rollback decision & execution | C | C | I | I | I | C | R | A | C | I |
| Incident triage | C | I | I | I | I | R | R | C | C | I |

> See [Release & Deployment Guide](./octoacme-release-and-deployment.md) for the full deployment checklist and rollback playbook.

---

## Phase 5: Retrospective & Continuous Improvement

| Activity | Project Mgr | Product Mgr | Business Analyst | Scrum Master | UX Designer | Developer | DevOps Engineer | Release Manager | Security Lead | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|
| Retrospective facilitation | C | I | I | A/R | I | R | I | I | I | I |
| Action item identification | C | C | C | R | C | R | C | C | C | I |
| Action item tracking & follow-up | A | I | I | R | I | I | I | I | I | I |
| Process improvement proposals | C | C | C | A/R | C | R | C | C | C | I |
| Metrics review (velocity, quality, incidents) | A | C | I | C | I | C | C | C | C | I |

> See [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) for templates and facilitation guidance.

---

## Quick-Reference: Role → Key Accountabilities

| Role | Primary Accountabilities Across Lifecycle |
|---|---|
| **Project Manager** | Initiation planning, risk register, stakeholder communication, delivery timelines |
| **Product Manager** | Backlog prioritization, acceptance criteria, product-market fit, sprint reviews |
| **Business Analyst** | Requirements elicitation, user stories, acceptance of delivered features |
| **Scrum Master** | Sprint ceremonies, blocker removal, velocity reporting, retrospective facilitation |
| **UX Designer** | UI/UX design, usability validation, UX handoff to Developers |
| **Developer** | Feature development, code/security review participation, smoke testing |
| **DevOps Engineer** | CI/CD pipelines, deployment execution, infrastructure, incident triage |
| **Release Manager** | Release go/no-go, deployment coordination, rollback decisions, release notes |
| **Security Lead** | Threat modeling, code security review, security sign-off, incident response |
| **Stakeholders** | Go/no-go approvals, requirements inputs, UAT sign-off, executive escalations |
