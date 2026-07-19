<p align="center">
  <a href="https://eshipjet.ai">
    <img src="https://eshipjet.ai/assets/logo.png" alt="EshipJet.ai" width="220">
  </a>
</p>

<h1 align="center">EShipJet</h1>

<p align="center">
  Enterprise shipping, logistics automation, carrier integrations, and AI-powered operational visibility.
</p>

<p align="center">
  <a href="https://eshipjet.ai">Website</a>
  ·
  <a href="https://github.com/Eshipjet-India-Pvt-Ltd">GitHub Organization</a>
  ·
  <a href="#platform">Platform</a>
  ·
  <a href="#projects">Projects</a>
  ·
  <a href="#developer-hub">Developer Hub</a>
  ·
  <a href="#qa-and-release">QA and Release</a>
</p>

---

## About

**EShipJet (ESJ)** builds commercial shipping, logistics, carrier-integration, enterprise automation, and operational visibility software for businesses that require reliable shipment processing, document handling, tracking, printing, and customer-specific deployment workflows.

Our products support controlled enterprise use across internal operations, customer implementations, partner integrations, and production shipping environments.

## Platform

EShipJet helps businesses manage:

| Area | Capabilities |
| --- | --- |
| Shipping operations | Shipment creation, rate shopping, shipping, voiding, labels, documents, and shipment history |
| Carrier integrations | FedEx, UPS, DHL, Forward Air, ATS, customer-specific carrier engines, and partner integrations |
| Tracking visibility | Scheduled tracking updates, webhook events, proof-of-delivery retrieval, and status synchronization |
| Enterprise configuration | Customer setup, business rules, user access, roles, integrations, and environment-specific behavior |
| Printer automation | ZPL, PDF, raw print support, Windows workstation printing, and label/document automation |
| Developer workflow | ESJ CLI, setup helpers, build commands, Git hooks, runbooks, and release guidance |

## Projects

Most EShipJet repositories are private and used for commercial product development, customer implementations, and controlled partner collaboration.

| Project | Purpose | Link |
| --- | --- | --- |
| ShipperCopilot 6.4 | Enterprise shipping application for shipment processing, carrier selection, label generation, and shipment lifecycle management | [SCOP-NGUI](https://github.com/Eshipjet-India-Pvt-Ltd/SCOP-NGUI) |
| SCOP-NGUI | Angular frontend for ShipperCopilot 6.4, including Ship Now, shipment history, dashboards, customer configuration, and environment-specific UI behavior | [Repository](https://github.com/Eshipjet-India-Pvt-Ltd/SCOP-NGUI) |
| SCOP-NODE-SERVICE | Backend service layer for shipment, customer, user, configuration, authentication, and integration workflows | [Repository](https://github.com/Eshipjet-India-Pvt-Ltd/SCOP-NODE-SERVICE) |
| SCOP-SCP-SERVICE | Carrier-processing service for rating, shipping, voiding, tracking, documents, and carrier API orchestration | [Repository](https://github.com/Eshipjet-India-Pvt-Ltd/SCOP-SCP-SERVICE) |
| Tracking Scheduler | Scheduler and webhook workflows for tracking updates, carrier events, POD retrieval, and status synchronization | [Repository](https://github.com/Eshipjet-India-Pvt-Ltd/scop-tracking-scheduler) |
| Printer Tools | Desktop printer utilities for ZPL, PDF, raw print support, and customer workstation deployment | [Repository](https://github.com/Eshipjet-India-Pvt-Ltd/printer) |
| ESJ CLI | Developer and release workflow tooling for setup, builds, hooks, branch guidance, and smoke tests | [Repository](https://github.com/Eshipjet-India-Pvt-Ltd/eshipjet-cli) |
| EShipJet Website | Public website for EshipJet.ai product and company presence | [Website](https://eshipjet.ai) |

## Developer Hub

Developers should start with the repository README and project documentation before making changes.

Recommended entry points:

- [EShipJet GitHub Organization](https://github.com/Eshipjet-India-Pvt-Ltd)
- [SCOP-NGUI README](https://github.com/Eshipjet-India-Pvt-Ltd/SCOP-NGUI/blob/shippercopilot-6.4-dev/README.md)
- [SCOP-NGUI Agent Instructions](https://github.com/Eshipjet-India-Pvt-Ltd/SCOP-NGUI/blob/shippercopilot-6.4-dev/AGENTS.md)
- [SCOP-NGUI Branches and Environments](https://github.com/Eshipjet-India-Pvt-Ltd/SCOP-NGUI/blob/shippercopilot-6.4-dev/docs/BRANCHES_AND_ENVIRONMENTS.md)
- [SCOP-NGUI Repository Structure](https://github.com/Eshipjet-India-Pvt-Ltd/SCOP-NGUI/blob/shippercopilot-6.4-dev/docs/REPOSITORY_STRUCTURE.md)
- [SCOP-NGUI Testing Guide](https://github.com/Eshipjet-India-Pvt-Ltd/SCOP-NGUI/blob/shippercopilot-6.4-dev/docs/testing/README.md)
- [ESJ CLI](https://github.com/Eshipjet-India-Pvt-Ltd/eshipjet-cli)

Standard SCOP-NGUI local workflow:

```bash
npm run esj -- install
npm run esj -- setup-hooks
npm run esj -- run
npm run esj -- guide
```

Build verification:

```bash
npm run esj -- build:ng
```

## QA and Release

Every production-impacting change should go through controlled review and tester sign-off before release.

QA sign-off should confirm:

- The assigned requirement or issue was tested
- The correct environment was used
- Regression areas were checked
- Carrier-specific behavior was verified where applicable
- Shipment, label, document, tracking, POD, and printer workflows were validated where applicable
- Evidence was attached where needed, including screenshots, shipment numbers, logs, or API traces
- Known limitations or pending items were documented

Recommended release controls:

- Confirm repository, branch, commit, and target environment
- Keep Dev, Demo, QAS, customer-specific, and Production lanes separate
- Run the relevant build and test commands
- Capture tester sign-off
- Document deployment evidence and rollback path
- Hand off customer-facing changes to support

## Wiki

The EShipJet project wiki should organize shared knowledge for engineering, QA, release, implementation, and support teams.

Recommended wiki menu:

| Section | Purpose |
| --- | --- |
| Project Portfolio | Repository ownership, project purpose, service map, and links |
| Developer Documentation | Setup, local run commands, code workflow, build verification, and PR checklist |
| QA and Tester Sign-Off | QA process, validation checklist, evidence expectations, and release sign-off template |
| Release and Deployment Governance | Environment lanes, deployment evidence, production controls, rollback, and support handoff |
| Carrier Integrations | Carrier workflow notes, API behavior, document rules, and troubleshooting |
| Customer Implementations | Customer-specific configuration, rollout notes, and support ownership |
| Support Runbook | Incident triage, escalation path, known issues, and recovery steps |

## Commercial Ownership

All repositories and source code under this organization are commercial, proprietary, and confidential unless explicitly stated otherwise.

```text
Copyright (c) 2026 EShipJet. All rights reserved.

This software is proprietary and confidential. Unauthorized copying,
distribution, modification, public sharing, sublicensing, or use of this
software is strictly prohibited without written permission from EShipJet.
```

## Contact

For business, implementation, support, or partnership inquiries, visit [EshipJet.ai](https://eshipjet.ai) or contact the official EShipJet team through approved company communication channels.

