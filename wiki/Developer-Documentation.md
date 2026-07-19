# Developer Documentation

Developer documentation must help an engineer set up, run, change, test, and safely release a project without relying on tribal knowledge.

## Required Documentation

Each repository should maintain:

- `README.md`
- `AGENTS.md`
- `docs/README.md`
- `docs/BRANCHES_AND_ENVIRONMENTS.md`
- `docs/REPOSITORY_STRUCTURE.md`
- `docs/testing/README.md`
- Deployment runbook
- Troubleshooting guide
- Release checklist

## SCOP-NGUI Developer Flow

```bash
npm run esj -- install
npm run esj -- setup-hooks
npm run esj -- run
npm run esj -- guide
```

Angular compile verification:

```bash
npm run esj -- build:ng
```

Test commands:

```bash
npm test
npm run test:coverage
npm run e2e:headless
```

## Branch and Environment Rules

- Dev work must stay in the Dev lane
- Demo work must stay in the Demo lane
- QAS work must stay in the QAS lane
- Customer-specific work must be clearly named and documented
- Production changes must have review, validation, and release sign-off

For SCOP-NGUI:

- Dev branch: `shippercopilot-6.4-dev`
- Demo branch: `shippercopilot-6.4-demo`

## Pull Request Checklist

Every pull request should include:

- Summary of the change
- Reason for the change
- Environment tested
- Commands run
- Screenshots or evidence for UI changes
- Shipment numbers or API evidence for shipping workflow changes
- Tester sign-off status
- Deployment notes
- Rollback considerations

## Documentation Quality Bar

Good documentation should:

- Name the exact environment
- Link to the repository, branch, PR, or runbook
- Include commands that can be copied and run
- Identify owners and reviewers
- Separate confirmed behavior from assumptions
- Avoid secrets, credentials, and customer-private data

