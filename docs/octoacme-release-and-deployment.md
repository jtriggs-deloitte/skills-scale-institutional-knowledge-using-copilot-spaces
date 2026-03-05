# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Key Roles in Release & Deployment
The following roles are actively involved during release. See [Roles & Personas](./octoacme-roles-and-personas.md) for full descriptions and [Responsibility Matrix — Phase 4](./octoacme-responsibility-matrix.md#phase-4-release--deployment) for RACI assignments.

- **Release Manager** — Owns the release process end-to-end: schedules deployment windows, chairs the go/no-go review, coordinates communications, and owns the rollback decision.
- **DevOps Engineer** — Executes deployment automation, confirms environment parity, and monitors system health post-deploy.
- **Security Lead** — Provides security sign-off before any production deployment; see [Security Review Checkpoint](./octoacme-handoff-checklist.md#2-security-review-checkpoint-execution--release).
- **Developer** — Confirms all acceptance criteria are met; supports smoke testing and incident triage.
- **Project Manager** — Coordinates stakeholder release communications.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (DevOps Engineer confirms)
- Security sign-off from Security Lead
- Release notes drafted (Release Manager + Product Manager)
- Rollback / mitigation plan documented and rehearsed (Release Manager + DevOps Engineer)
- Smoke tests prepared
- See [Release Readiness Checklist](./octoacme-handoff-checklist.md#3-release-readiness-execution--release--deployment) for the full pre-release gate

## Deployment Checklist
- [ ] Go/No-Go meeting held (Release Manager, Project Manager, Product Manager, Security Lead)
- [ ] Security sign-off confirmed (Security Lead)
- [ ] Deployment window scheduled (Release Manager + DevOps Engineer)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests (DevOps Engineer + Developer)
- [ ] Deploy to production (automated pipeline preferred; DevOps Engineer executes)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support (Project Manager + Release Manager)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Release Manager makes the rollback call; DevOps Engineer executes
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - For security incidents, immediately notify Security Lead and follow the security incident runbook
  - Triage root cause and capture action items; schedule blameless retrospective

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
