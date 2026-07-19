# Release and Deployment Governance

EShipJet releases must keep environments, branches, customer lanes, and production deployments clearly separated.

## Environment Lanes

Use explicit environment names in commits, PRs, test notes, release notes, and support handoffs.

- Dev
- Demo
- QAS
- Customer-specific lane
- Production

## Release Checklist

Before release:

- [ ] Correct branch confirmed
- [ ] Correct environment confirmed
- [ ] Pull request reviewed
- [ ] Build completed
- [ ] Unit or focused tests completed
- [ ] Browser or workflow validation completed where needed
- [ ] QA tester sign-off completed
- [ ] Deployment runbook followed
- [ ] Release notes prepared
- [ ] Rollback path identified

## Deployment Evidence

Every release should capture:

- Repository
- Branch
- Commit SHA
- Build or workflow run
- Deployment target
- Environment
- Deployed by
- Deployment time
- Smoke-test result
- Known issues or exceptions

## Production Release Controls

Production releases require:

- Business or release approval
- QA sign-off
- Engineering owner confirmation
- Deployment owner confirmation
- Support handoff when customer-facing behavior changes

## Rollback Plan

Every production release should identify:

- Last known good version
- Rollback command or deployment action
- Database or configuration impact
- Customer communication owner
- Validation steps after rollback

## Support Handoff

Support handoff should include:

- What changed
- Which customers are affected
- What symptoms the change resolves
- How to validate the fix
- Known limitations
- Escalation owner

