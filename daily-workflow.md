# Daily Workflow

The full daily loop for the Service Coordinator, from shift start through the scheduling decision and back into ongoing queue monitoring.

```mermaid
flowchart TD
    A([Shift start]) --> B[Morning board cleanup<br/><i>Review & clean up boards</i>]
    B --> C[New ticket received<br/><i>Portal, email, phone, alert</i>]
    C --> D[Clarify summary<br/><i>Confirm issue details</i>]
    D --> E[Determine correct board<br/><i>Which board it belongs on</i>]
    E --> F[Select agreement<br/><i>Match client contract / SLA</i>]
    F --> G[Assign & route ticket<br/><i>Named tech, correct queue</i>]
    G --> H{Scheduling<br/>needed?}
    H -- Yes --> I[Schedule call<br/><i>Confirm date, time & scope</i>]
    I --> J[Update & confirm<br/><i>Log in ticket & notify tech</i>]
    J --> K[Monitor queue<br/><i>Repeat throughout shift</i>]
    H -- No --> K
    K -. next ticket .-> C
    K -. possible P1 .-> P[[Major Incident process]]

    classDef intake fill:#eef,stroke:#55c,color:#222
    classDef sched fill:#fdeee8,stroke:#d65,color:#222
    classDef neutral fill:#f2f2f2,stroke:#888,color:#222
    class C,D,E,F,G intake
    class I,J sched
    class B,K neutral
```

A static image version is in [`daily-workflow.png`](daily-workflow.png).
