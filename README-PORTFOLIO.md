# Portfolio build

This repository is a redacted portfolio representation of a procurement workflow.

## What this demonstrates

- Process discovery and as-is / to-be analysis
- Business requirements and acceptance criteria
- Stakeholder and responsibility mapping
- Workflow controls and approval routing
- Exception management
- UAT traceability
- Risk and decision management
- Technical architecture
- Working browser prototype
- Audit-oriented workflow history

## Prototype flow

**Request → validation → specification review → approval → tender readiness → exception handling → audit**

Open the prototype and move a request through its workflow states.

## Technical scope

The prototype uses a lightweight browser implementation so the workflow can be inspected without a backend dependency. Production architecture would introduce authenticated identity, persistent storage, document management, notifications, supplier controls and policy-based access.

## Evidence

- [`docs/`](./docs) — project analysis and delivery artefacts
- [`architecture/`](./architecture) — system view
- [`app/`](./app) — working prototype
- [`docs/13-build-evidence.md`](./docs/13-build-evidence.md) — implementation scope and test path

## Data boundary

All visible records are synthetic. No live tender, supplier, pricing or confidential government information is included.

## Project framing

This is presented as a **digital transformation / project delivery case study with a working prototype**, not as a claim that the production procurement platform is reproduced in this repository.
