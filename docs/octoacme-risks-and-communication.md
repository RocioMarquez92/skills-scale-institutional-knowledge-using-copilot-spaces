# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

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
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support, design, QA)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- Release Manager coordinates deployment communications
- Support Engineer provides production health updates
- UX/UI Designer shares design reviews and usability findings
- QA Lead reports on quality metrics and testing progress

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary (prepared by Support Engineer or Release Manager)
- Actions being taken
- Expected timeline
- Stakeholder notifications (coordinated by Release Manager)
- Post-incident blameless retrospective scheduled (led by Release Manager)

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
- For quality concerns: Developer -> QA Lead -> PM -> Product Lead
- For release issues: Developer/QA Lead -> Release Manager -> PM -> Product Lead
- For production incidents: Support Engineer -> Release Manager -> PM -> Product Lead
- For design conflicts: Developer -> UX/UI Designer -> Product Manager -> Product Lead

## Role-Specific Communication Responsibilities
- **Project Manager**: Weekly status updates, risk register, stakeholder briefings
- **QA Lead**: Quality reports, test coverage metrics, bug triage outcomes
- **Release Manager**: Release schedules, deployment announcements, release retrospectives
- **Support Engineer**: Incident reports, production health updates, user feedback summaries
- **UX/UI Designer**: Design reviews, usability testing results, accessibility reports
- **Product Manager**: Product vision, roadmap updates, prioritization decisions
- **Developers**: Technical design docs, PR descriptions, code review feedback
