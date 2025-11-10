# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies (facilitated by Scrum Master)
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone
- Design reviews (as needed with UX Designer)
- Security reviews (as needed with Security Lead)
- Data/metrics reviews (weekly or bi-weekly with Data Analyst)

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI (reviewed by Security Lead)
- Accessibility testing for user-facing features (coordinated with UX Designer)
- Manual QA for feature acceptance when needed
- Usability testing for significant UX changes (led by UX Designer)

## Reporting & Metrics
- Track velocity and burndown (maintained by Scrum Master)
- Monitor success metrics identified in the Project One-pager (tracked by Data Analyst)
- Use dashboards for key signals (errors, latency, usage)
- Review user feedback and support trends (from Support Engineers)
- Track security vulnerabilities and remediation (monitored by Security Lead)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Security scanning enabled in CI pipeline
- [ ] Analytics instrumentation implemented and validated
- [ ] Accessibility testing integrated for UI changes
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Support team briefed on upcoming changes
- [ ] UX research and validation completed for user-facing features
