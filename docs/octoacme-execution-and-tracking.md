# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
  - QA Lead reviews test coverage for critical features
  - Move to QA column for validation before marking Done

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed
- QA Lead reviews test strategy and validates quality gates
- UX/UI Designer validates usability for user-facing features
- Accessibility testing coordinated by UX/UI Designer

## Reporting & Metrics
- Track velocity and burndown (Project Manager)
- Monitor success metrics identified in the Project One-pager (Product Manager)
- Use dashboards for key signals (errors, latency, usage) (Support Engineer monitors)
- QA Lead reports on test coverage, defect trends, and quality metrics
- Release Manager tracks deployment frequency and success rates
- UX/UI Designer monitors user satisfaction and usability metrics

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM or QA Lead escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues
- For release blockers: Release Manager coordinates with QA Lead and PM
- For production incidents: Support Engineer follows incident escalation path

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] QA Lead assigned and test strategy defined
- [ ] Release Manager identified for deployment coordination
- [ ] Support Engineer prepared for production monitoring
