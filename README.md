# Diagrams

Generic, illustrative diagrams of how I approach documentation work. GitHub renders Mermaid automatically.

---

## 1. Document lifecycle

```mermaid
stateDiagram-v2
    [*] --> Draft
    Draft --> Review: Author submits
    Review --> Draft: Changes requested
    Review --> Approved: Approver signs off
    Approved --> Published: Posted to single source of truth
    Published --> ScheduledReview: Review date reached
    Published --> Draft: Process change
    ScheduledReview --> Published: Still accurate
    ScheduledReview --> Draft: Update needed
    Published --> Retired: Superseded
    Retired --> [*]
```

---

## 2. Audit & disposition process

```mermaid
flowchart TD
    A[Inventory all documents] --> B[Assess each document]
    B --> C{Accurate &<br/>current?}
    C -- Yes --> D{Owned &<br/>versioned?}
    D -- Yes --> K[Keep]
    D -- No --> K2[Keep + add<br/>control blocks]
    C -- No --> E{Overlaps with<br/>another doc?}
    E -- Yes --> F[Consolidate]
    E -- No --> G{Still a<br/>needed process?}
    G -- Yes --> H[Update / rewrite]
    G -- No --> R[Retire]
    I[Gap found:<br/>no document exists] --> J[Create new]
    F --> X[Cross-document<br/>reconciliation]
    H --> X
    J --> X
    K2 --> X
    X --> P[Review, approve, publish]
```

---

## 3. Documentation hierarchy

How the document types relate, from broad to specific.

```mermaid
flowchart TD
    P[Policy / Standard<br/><i>What must be true</i>] --> S[SOP<br/><i>How to do it, in full</i>]
    S --> W[Workflow<br/><i>Decision path</i>]
    S --> Q[Quick Reference<br/><i>Do it under pressure</i>]
    S --> T[Training Program<br/><i>Learn to do it</i>]
    M[Roles & Career Matrix<br/><i>Who does it</i>] --> S
```

---

## 4. Generic tiered escalation model

An illustrative, industry-standard model. It does not represent any specific organization's procedure.

```mermaid
flowchart LR
    U([Request / Incident]) --> L1[L1 Support<br/>Triage & resolve]
    L1 -- Resolved --> C([Close])
    L1 -- Needs escalation --> D{Escalation<br/>criteria met?}
    D -- No --> L1
    D -- Yes --> L2[L2 Support<br/>Named owner]
    L2 -- Resolved --> C
    L2 -- Needs escalation --> E[Engineering<br/>Named owner]
    E --> C
```

> **Design principle:** every escalation is a direct handoff to a named owner, and the ticket's documentation must be complete before it moves.
