# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

For a full view of how these roles interact across the project lifecycle, see [Responsibility Matrix](./octoacme-responsibility-matrix.md) and the [Handoff & Communication Checklist](./octoacme-handoff-checklist.md).

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

### Key Interactions
- Receives requirements from Business Analyst and Product Manager
- Coordinates with UX Designer on UI implementation details
- Escalates infrastructure blockers to DevOps Engineer
- Works with Security Lead on secure coding practices
- Notifies Release Manager when features are ready for deployment

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with Project Manager and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

### Key Interactions
- Partners with Business Analyst to refine requirements and user stories
- Aligns with UX Designer on product vision and usability findings
- Coordinates with Project Manager on backlog priorities and timelines
- Reviews risk reports from Security Lead

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

### Key Interactions
- Works with Scrum Master to coordinate sprint planning and retrospectives
- Aligns with Release Manager on release schedules and deployment windows
- Escalates blockers raised by Scrum Master or DevOps Engineer
- Communicates project status to Stakeholder groups

---

## Scrum Master

### Role Summary
The Scrum Master facilitates agile ceremonies, removes impediments, and coaches the team on continuous improvement. They serve as a process guardian and enabler, ensuring the team can work effectively sprint over sprint.

### Responsibilities
- Facilitate daily standups, sprint planning, sprint reviews, and retrospectives
- Identify and remove blockers that impede team velocity
- Coach the team on agile practices and process improvement
- Shield the team from unplanned interruptions during a sprint
- Track and report sprint health metrics (velocity, burndown)

### Goals
- Maximize team throughput and predictability
- Foster a culture of continuous improvement
- Reduce process friction and recurring blockers

### Typical Communication
- Daily standups and sprint ceremonies
- Retrospective action item tracking
- Impediment log and escalation notes

### Key Interactions
- Coordinates sprint planning and retrospectives with Project Manager
- Supports Developers in surfacing and resolving blockers
- Advises Product Manager on realistic backlog sizing and sprint capacity
- Escalates systemic issues to Project Manager or Product Manager as needed

---

## UX Designer

### Role Summary
UX Designers create user interface designs, conduct usability reviews, and ensure product experiences align with the product vision and user needs. They bridge user insights and technical implementation.

### Responsibilities
- Design wireframes, prototypes, and high-fidelity UI assets
- Conduct usability reviews and user research sessions
- Maintain a design system or component library
- Collaborate with Developers to validate UI implementation
- Provide input on release readiness from a UX perspective

### Goals
- Deliver intuitive, accessible, and visually consistent experiences
- Reduce rework by catching UX issues early in the design phase
- Ensure the product vision is faithfully translated into the UI

### Typical Communication
- Design reviews and prototype walkthroughs
- Handoff notes to Developers (annotated designs, component specs)
- Feedback during sprint reviews

### Key Interactions
- Collaborates with Product Manager to understand requirements and user goals
- Hands off designs and specifications to Developers for implementation
- Participates in sprint reviews to validate UI against acceptance criteria
- Contributes to the [Handoff & Communication Checklist](./octoacme-handoff-checklist.md) at UX sign-off gates

---

## Release Manager

### Role Summary
Release Managers oversee build and deployment pipelines, coordinate release schedules, and ensure rollback and incident protocols are documented and rehearsed. They are the final gate before production deployment.

### Responsibilities
- Manage and approve release schedules and deployment windows
- Ensure all pre-release criteria are met before promoting builds
- Coordinate release communications with stakeholders
- Maintain and rehearse rollback and incident response protocols
- Track release readiness across teams

### Goals
- Enable predictable, low-risk releases to production
- Minimize production incidents caused by deployment failures
- Maintain a clear and auditable release history

### Typical Communication
- Release readiness reviews and go/no-go meetings
- Release notes and stakeholder notifications
- Post-release incident reports

### Key Interactions
- Aligns with Developers and Project Manager on technical readiness
- Coordinates with DevOps Engineer on pipeline health and deployment automation
- Consults with Security Lead to confirm security sign-off before release
- Communicates deployment status and outcomes to Stakeholders
- See [Release & Deployment Guide](./octoacme-release-and-deployment.md) for detailed release process

---

## DevOps Engineer

### Role Summary
DevOps Engineers maintain CI/CD pipelines, infrastructure-as-code, and system health monitoring. They enable fast, reliable delivery by automating build, test, and deployment workflows.

### Responsibilities
- Build and maintain CI/CD pipelines and deployment automation
- Manage infrastructure-as-code and environment configuration
- Monitor system health, alerts, and on-call response
- Support incident triage and post-incident remediation
- Optimize pipeline performance and reliability

### Goals
- Reduce deployment lead time and failure rate
- Ensure environment parity between staging and production
- Provide observability into system performance and incidents

### Typical Communication
- Pipeline status alerts and deployment dashboards
- Incident reports and post-mortems
- Infrastructure change notifications

### Key Interactions
- Partners with Developers to resolve build and environment blockers
- Coordinates with Release Manager on deployment automation and windows
- Reports deployment status and incidents to Project Manager and Product Manager
- Collaborates with Security Lead on secure infrastructure and compliance controls
- See [Execution & Tracking](./octoacme-execution-and-tracking.md) for CI/CD workflow standards

---

## Business Analyst

### Role Summary
Business Analysts elicit and clarify requirements, model workflows, and help validate business value. They act as the bridge between stakeholders and the delivery team.

### Responsibilities
- Facilitate requirements workshops with stakeholders
- Document functional requirements, user stories, and acceptance criteria
- Model current-state and future-state business workflows
- Validate that delivered solutions meet business objectives
- Assist in identifying and managing scope changes

### Goals
- Ensure requirements are complete, clear, and testable
- Reduce rework caused by misunderstood requirements
- Align delivery team output with stakeholder expectations

### Typical Communication
- Requirements walkthroughs and review sessions
- User story mapping and acceptance criteria documentation
- Scope change requests and impact assessments

### Key Interactions
- Works with Product Manager and Stakeholders to define and refine requirements
- Supports Project Manager in capturing deliverables and managing scope
- Assists Developers in interpreting user stories and edge cases
- Contributes inputs to the [Handoff & Communication Checklist](./octoacme-handoff-checklist.md) during planning

---

## Security Lead

### Role Summary
The Security Lead reviews code, processes, and infrastructure for compliance and vulnerability risks. They lead incident response for security events and guide the team in secure development practices.

### Responsibilities
- Review code, architecture, and third-party dependencies for security vulnerabilities
- Define and maintain secure development standards and guidelines
- Lead security incident response and post-incident reviews
- Conduct or facilitate security assessments (threat modeling, penetration testing)
- Ensure compliance with relevant regulations and internal policies

### Goals
- Reduce the attack surface and vulnerability exposure of OctoAcme systems
- Foster a security-first engineering culture
- Ensure timely detection and remediation of security incidents

### Typical Communication
- Security findings and remediation advisories
- Risk reports to Product Manager and Project Manager
- Incident response notifications and post-mortem write-ups

### Key Interactions
- Consults with Developers on secure coding practices and vulnerability fixes
- Provides security sign-off to Release Manager before production deployments
- Reports security risks to Project Manager and Product Manager via the Risk Register
- Collaborates with DevOps Engineer on secure infrastructure configuration
- See [Risk Management & Communication](./octoacme-risks-and-communication.md) for escalation paths

---

## Stakeholders

### Role Summary
Stakeholders represent the business, customer, and organizational interests in a project. They provide direction, funding, and approval authority, and consume project outputs. Different stakeholder subtypes have distinct communication and decision-making needs.

### Stakeholder Subtypes

#### Executive Sponsor
- **Role**: Ultimate decision-maker and champion for the project at the leadership level.
- **Inputs**: Business case, high-level milestones, budget approvals.
- **Approvals**: Go/no-go for major phases, budget changes, scope escalations.
- **Communication cadence**: Monthly or milestone-based briefings; immediate notification for critical risks.

#### Business Owner / Product Sponsor
- **Role**: Owns the business outcome and validates that delivery meets business objectives.
- **Inputs**: Success metrics, business requirements, prioritization guidance.
- **Approvals**: Acceptance of delivered features, sign-off on release readiness.
- **Communication cadence**: Sprint reviews, weekly status updates.

#### End Users / User Representatives
- **Role**: Represent the people who will use the product; provide usability feedback.
- **Inputs**: User feedback, usability testing participation, acceptance testing.
- **Approvals**: User acceptance testing (UAT) sign-off.
- **Communication cadence**: User research sessions, sprint demos, beta releases.

#### Compliance / Legal
- **Role**: Ensure the project meets regulatory, legal, and policy requirements.
- **Inputs**: Compliance requirements, legal constraints, policy guidelines.
- **Approvals**: Sign-off on data handling practices, terms of service, regulatory compliance.
- **Communication cadence**: Milestone reviews for compliance-sensitive deliverables.

### Goals
- Ensure the project delivers measurable business and user value
- Provide timely decisions to unblock delivery
- Maintain confidence in project progress and risk posture

### Typical Communication
- Milestone briefings and executive status reports
- Sprint reviews and demos
- Risk and decision escalation notifications

### Key Interactions
- Provide requirements inputs to Business Analyst and Product Manager
- Receive project status from Project Manager
- Participate in release readiness reviews coordinated by Release Manager
- Escalation target for Project Manager when scope or budget changes are required

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Responsibility Matrix](./octoacme-responsibility-matrix.md) for a lifecycle-phase view of role assignments.
- See [Handoff & Communication Checklist](./octoacme-handoff-checklist.md) for actionable cross-role coordination templates.

