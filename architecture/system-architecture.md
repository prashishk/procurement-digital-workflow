# System architecture

```mermaid
flowchart LR
  U[Requesting unit] --> W[Workflow]
  W --> V[Validation and readiness]
  V --> R[Specification review]
  R --> A[Approval routing]
  A --> T[Tender readiness]
  W --> E[Exception handling]
  A --> AU[Audit history]
  T --> AU
```

**Production boundary:** authentication, persistent storage, document storage, notifications, supplier controls and policy-based access would sit behind the prototype workflow. All demo records are synthetic.