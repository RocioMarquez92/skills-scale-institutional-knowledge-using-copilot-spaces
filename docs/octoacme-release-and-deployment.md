# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- QA Lead sign-off on quality gates and testing completion
- Release notes drafted by Release Manager
- Rollback / mitigation plan documented
- Smoke tests prepared and validated by QA Lead

## Deployment Checklist
- [ ] Deployment window scheduled by Release Manager (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests (QA Lead validates)
- [ ] Go/no-go decision with QA Lead and Release Manager
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications with QA Lead
- [ ] Release Manager announces release to stakeholders
- [ ] Support Engineer notified and prepared for monitoring

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Release Manager triggers incident response and notifies on-call
  - Support Engineer monitors production health and user impact
  - Rollback to last known-good release if necessary (Release Manager coordinates)
  - QA Lead validates rollback and post-rollback testing
  - Triage root cause and capture action items
  - Release Manager leads post-incident retrospective

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
- Prepared by: Release Manager
- Quality sign-off: QA Lead

## Roles in Release Process
- **Release Manager**: Orchestrates the entire release process, coordinates timing, prepares release notes, and leads retrospectives
- **QA Lead**: Validates quality gates, signs off on testing completion, and confirms go/no-go decisions
- **Support Engineer**: Monitors production health post-release, responds to incidents, and provides feedback on release quality
- **Project Manager**: Ensures release aligns with project timeline and stakeholder expectations
- **Developers**: Support deployment, troubleshooting, and hotfixes as needed
