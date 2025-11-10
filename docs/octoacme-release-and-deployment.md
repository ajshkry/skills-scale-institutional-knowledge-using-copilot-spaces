# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (validated by Security Lead)
- Release notes drafted (with input from Support Engineers)
- Rollback / mitigation plan documented
- Smoke tests prepared
- Analytics instrumentation verified (by Data Analyst)
- Accessibility compliance checked for UI changes (by UX Designer)
- Support team trained and documentation updated

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Security scan completed with no critical issues
- [ ] Support team briefed on changes and known issues
- [ ] Deploy to staging and run smoke tests
- [ ] Verify analytics and monitoring instrumentation
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Confirm metrics and alerts are functioning
- [ ] Announce release to stakeholders and support
- [ ] Update support documentation and FAQs

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (including Security Lead if security-related)
  - Rollback to last known-good release if necessary
  - Alert Support Engineers to handle customer communications
  - Triage root cause and capture action items
  - Schedule blameless post-mortem with relevant team members

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
