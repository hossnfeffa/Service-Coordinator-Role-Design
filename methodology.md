# SOP Audit & Modernization Methodology

A repeatable framework for bringing an operational documentation set up to date.

---

## Phase 1: Inventory

Build a complete list before changing anything.

- [ ] Collect every SOP, workflow, policy, cheat sheet, and onboarding artifact, in any format
- [ ] Record each document's format, last-modified date, owner (if any), and location
- [ ] Flag duplicates and multiple versions of the same topic
- [ ] Note "shadow documentation": spreadsheets, chat posts, and personal notes that people actually rely on

**Output:** a documentation tracker with one row per topic.

## Phase 2: Assessment

Score each document against five questions:

| Question | Red flag |
| --- | --- |
| **Accurate?** Does it match how the work is done today? | References retired roles, tools, or workflows |
| **Complete?** Could a new hire follow it without help? | Missing steps, assumed knowledge |
| **Consistent?** Does it agree with related documents? | Conflicting instructions or terminology |
| **Owned?** Is there a named owner and approver? | Blank ownership, no revision history |
| **Usable?** Is it the right format for when it's used? | A 10-page document needed mid-incident |

## Phase 3: Standardize first

Settle the standards **before** rewriting, so every document doesn't have to be revised twice.

- Canonical terminology (roles, tiers, priorities, statuses)
- Standard document structure (see [documentation-standards.md](documentation-standards.md))
- Visual conventions (callouts, step formatting, notes)
- Version numbering and revision-history format

## Phase 4: Disposition

Decide one action per document:

| Action | When to use it |
| --- | --- |
| **Keep** | Accurate and well-structured; only needs ownership and revision blocks |
| **Update** | Structure is sound but content is outdated |
| **Consolidate** | Two or more documents cover the same topic |
| **Create** | A role or recurring scenario has no documentation |
| **Split** | One document serves two audiences; create a full SOP plus a quick reference |
| **Retire** | Superseded by a newer document; archive it so no one uses it by mistake |

## Phase 5: Build

- Interview or observe the people doing the work. Document reality, not theory.
- Write the full SOP first, then distill a quick reference from it.
- Use numbered steps for sequences, and decision points for branches.
- Put warnings exactly where the risk occurs, not in a section at the end.

## Phase 6: Cross-document reconciliation

When a document changes, ask: *what else references this?*

- Role changes → career matrix, responsibilities, expectations, training program
- Process changes → quick references, workflows, onboarding material
- Contact changes → every cheat sheet and transfer procedure

Log any knock-on gaps in the tracker as open items.

## Phase 7: Control & maintain

- Assign an **owner** (keeps it accurate) and an **approver** (signs off on changes)
- Add a **revision history** table
- Publish to a single, known location
- **Retire** superseded versions explicitly
- Schedule a **review date**
