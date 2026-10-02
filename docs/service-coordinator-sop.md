# Service Coordinator SOP

| | |
|---|---|
| **Document type** | Standard Operating Procedure |
| **Role** | Service Coordinator |
| **Owner** | Service Desk Supervisor |
| **Version** | 1.0 |

---

## Purpose

This document describes the day-to-day process for the Service Coordinator role: keeping the service boards clean, triaging and routing incoming tickets, and coordinating scheduling with clients. It sets the expectation for how a ticket should look, and where it should land, before it is handed off to a technician.

## Scope

This covers the full daily workflow for anyone working the Service Coordinator seat during business hours.

**Out of scope:** after-hours and on-call handling. Those are covered by separate On-Call and Major Incident (P1) procedures.

## Resources

- **PSA / ticketing platform** (e.g., ConnectWise Manage)
  - **Dispatch Portal:** shows scheduled tickets, activities, and technician utilization
  - **Calendar:** used to manage appointments
- **Access-management platform:** logins and security roles
- **Reporting platform** (e.g., BrightGauge): KPI dashboards and reporting
- **Team chat channels:**
  - Service Desk – General
  - Service Desk – per-tier channels (L1 / L2 / SE)
  - Impact Notification (urgent pickups)
  - Field Engineers

---

## Process

### 1. Morning Board Cleanup

→ Review all assigned boards at the start of the shift, before taking new calls or tickets.

→ Close or update any ticket left in a stale or incorrect status by the prior shift.

→ Confirm the new-ticket board is clear and note who is next in the rotation.

→ Post in the L1 channel if anything from overnight needs another team member's attention.

### 2. Ticket Intake & Triage

→ New tickets arrive through the client portal, email-to-ticket, the phone queue, or an automated alert.

→ Read the full ticket, including any attachments, before taking action.

→ **Clarify the summary.** It must state:
   - who is impacted
   - the expected behavior compared with the observed behavior
   - the change required

→ Confirm the contact is the real point of contact for this issue, not just whoever the ticket happened to come in from.

→ **Determine the correct board:** Service Desk L1, L2, Systems Engineers (SE), Engineering, or Voice. If it isn't clear, ask a senior team member rather than guess.

→ **Select the agreement** that matches the work being done. The PSA sets a default. Review it critically instead of accepting it automatically.

→ Assign and route the ticket to the correct board, then confirm it saves cleanly.

> **Tip:** A ticket that leaves triage with a clear summary, the correct contact, the correct board, and the correct agreement saves the technician time, keeps billing accurate, and keeps SLA reporting clean.

### 3. Dispatching & Scheduling

→ Before assigning a ticket, check technician schedules and utilization in the **Dispatch Portal**. It shows team and individual utilization bars, color-coded by schedule type.

→ **Match by fit, not by availability.** Match the ticket to a technician by skill, certification, and familiarity with that client's environment, not just whoever happens to be free.

→ **Balance workload across the team.** Don't send every ticket to the most senior technician just because a client asks for them by name. Spreading work evenly keeps your strongest technicians from burning out.

→ When a ticket needs an appointment, call the client to confirm a date and time that works for both them and the assigned technician.

→ Confirm scope on the call: what work is being done and roughly how long it should take.

→ Drag the ticket into the technician's open slot on the Dispatch Portal. If you're moving a ticket that is already scheduled, send a Status Request with the relevant details; it is logged automatically in the ticket's internal notes.

→ If no technician is available yet for an urgent issue, post the ticket in the **Impact Notification** channel, when appropriate, so an available technician can pick it up.

→ **Technician out of office:** review their board and reassign tickets based on need. Ask whether it must be solved today, whether the client has responded, and whether it's time-sensitive. Not everything needs to move, so use judgment.

→ Notify the assigned technician of the scheduled appointment, and log the confirmed date, time, and notes directly in the ticket.

→ Follow up on completed appointments and compare the actual time against what was scheduled. This feeds SLA and utilization reporting.

> **Warning:** Every ticket must end up assigned to a **named person**. Never leave work sitting on an unassigned resource.

### 4. Ongoing Queue Monitoring

→ Keep monitoring the boards throughout the shift, not just at the start and end.

→ Re-triage any ticket that has sat without movement or without a clear owner.

→ Escalate anything that looks like it could be a P1 to the **Major Incident process** instead of handling it as a standard ticket.

---

## Workflow at a Glance

See [`../diagrams/daily-workflow.md`](../diagrams/daily-workflow.md) for the full daily loop, from shift start through the scheduling decision and back into ongoing queue monitoring.

## Onboarding

New Service Coordinators ramp up in three phases. See [`onboarding-plan.md`](onboarding-plan.md).

---

## Ownership

| Owner | Title | Date |
|-------|-------|------|
| _TBD_ | Service Desk Supervisor | _TBD_ |

## Revision History

| Version | Description | Revision Date | Reviewer / Approver |
|---------|-------------|---------------|---------------------|
| 1.0 | Initial version | | |
