# Design Decisions

Why the Service Coordinator role and its process are built the way they are.

---

### 1. A dedicated role between intake and technicians

**Decision:** Triage, routing, and scheduling belong to one owner instead of being spread across whichever technician picks up the ticket.

**Why:** When everyone triages, nobody owns ticket quality. A single coordinator applies one standard to every ticket and gives the desk one place to look when something is misrouted.

### 2. A required ticket summary format

**Decision:** Every summary must state who is impacted, the expected behavior compared with the observed behavior, and the change required.

**Why:** Technicians shouldn't have to re-interview the client. A structured summary also makes tickets searchable and reportable later.

### 3. Agreements are reviewed, not defaulted

**Decision:** The coordinator checks the contract agreement on every ticket instead of accepting the system default.

**Why:** The wrong agreement leads to billing errors, the wrong SLA clock, and misleading profitability data. That's a small check up front that prevents expensive cleanup later.

### 4. Assign by fit and balance workload

**Decision:** Tickets are matched by skill, certification, and familiarity with the client's environment, and workload is deliberately spread across the team, even when a client asks for a specific technician.

**Why:** Assigning by availability alone produces poor first-time fix rates. Assigning by client request alone burns out the most senior technicians and keeps others from growing.

### 5. Hard handoff to a named person

**Decision:** Tickets are assigned directly to a named technician. Nothing waits in an unassigned queue.

**Why:** Pull-based queues let work sit without an owner. Direct assignment makes accountability and SLA tracking clear.

### 6. Scheduling closes the loop

**Decision:** After an appointment, the coordinator compares the actual time against the scheduled time.

**Why:** This keeps utilization and SLA reporting accurate, and it improves how future appointments are scoped.

### 7. Use judgment when technicians are out

**Decision:** When a technician is out, their board is reviewed and reassigned based on need, not moved wholesale.

**Why:** Moving everything creates churn and confuses clients. Moving only time-sensitive or client-responsive work keeps continuity where it matters.

### 8. P1s leave the standard process

**Decision:** Anything that looks like a possible major incident is escalated to the Major Incident process immediately.

**Why:** Handling a P1 like a standard ticket costs response time. The coordinator's job is to spot it and hand it off, not to work it.

### 9. Onboarding with measurable criteria

**Decision:** Each onboarding phase has explicit success criteria, such as 90% of tickets assigned within the SLA window and about 95% of escalations routed correctly.

**Why:** "They seem ready" isn't a standard. Measurable gates make readiness objective and give new hires a clear target.
