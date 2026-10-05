# 06 — Logical Architecture

```mermaid
flowchart LR
  U[Users & Approvers] --> W[Workflow & Case Management]
  W --> V[Validation & Rules]
  W --> D[Document / Evidence Store]
  W --> A[Audit Event Store]
  W --> N[Notifications]
  W --> I[Tender / External Integrations]
  V --> AI[AI Assist Layer]
  AI --> W
  R[Reporting & Analytics] --> A
  R --> W
```

## Architecture Principles

- workflow state is authoritative
- policy rules remain deterministic where possible
- AI outputs are advisory and reviewable
- evidence is linked to decisions
- integrations are isolated behind controlled interfaces
- audit events are append-oriented and tamper-evident where required

## Security Model

**Identity → RBAC → Workflow authorisation → Data access → Audit**

Sensitive data should be minimised, encrypted and exposed only to roles with a legitimate business need.
