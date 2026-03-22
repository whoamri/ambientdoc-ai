# AmbientDoc — AI-First OS Gap Scan

_Scanned: 2026-03-22_

---

## Raw Data

### LINEAR

- Project: `AmbientDoc` (team: AMDOC / key: AMD)
- Status: **Backlog** — despite being live in production for 14 months
- Lead: **unassigned** (empty)
- Initiatives: none linked
- Milestones: none
- Gate criteria: none documented
- Only issue: AMD-5 "AmbientDoc Pilot" — High priority, Backlog, created by Amri Abuseman 2026-03-22, no owner

### GITHUB (`whoamri/ambientdoc-ai`, main)

- 1 commit: "Initial commit" — 2026-03-22
- Contents: LICENSE only
- No `/evals/` directory
- No prompt files, no model versioning, no gate review records
- No code whatsoever

### SLACK (`#ambient-doc-feedback`, last 14 days)

- Channel created: 2026-03-22
- 3 messages, 1 unique user (physician)
  - "notes feel different this week... less precise on the assessment section"
  - "medication dosage was listed differently than what I said. I caught them on review but it's adding time, not saving it."
  - "Third day of this now. Is anyone actually monitoring the system? Should I be filing an incident report somewhere?"
- No response from engineering or leadership
- No incident ticket created

---

## Four-Layer Gap Scan

| Layer | Finding | Gap |
|---|---|---|
| **THE MAP** | Linear project exists but status is "Backlog" — not reflected as live/active | Registry doesn't match reality; no stage documented |
| **THE OWNERS** | Lead field empty; AMD-5 has no assignee | No named person accountable for behavioral outcomes |
| **THE GATES** | No milestones, no gate criteria, no review linked to any model change | CMO committed 90-day scale with zero written gate criteria |
| **THE PULSE** | Physician reporting dosage errors for 3 days; zero response; no review triggered | No event triggers, no scheduled review, no escalation path |

---

## Portfolio Table

| Initiative | Stage | Owner | Next Gate | Risk Flag | Tier |
|---|---|---|---|---|---|
| AmbientDoc | Pilot → Scale (pressure) | Unassigned | Scale Gate: undefined | **HIGH** | 1 |

---

## Signal Recommendation

AmbientDoc cannot move to Scale. A physician is actively reporting medication dosage errors in AI-generated notes — three days running, with no acknowledgment — and no one owns the system's clinical output quality. The Linear project is miscategorized as Backlog despite being live in production. The GitHub repo has no code, no evals, and no record of any model or prompt change, even though NorthBridge does not control the underlying MedScribe model and either party can update it without review. Before scaling from 3 to 40 physicians, NorthBridge must:

- [ ] Assign a named clinical AI owner accountable for output quality
- [ ] Define and document Scale gate criteria including a minimum eval baseline and a model-change review process
- [ ] Triage the active Slack quality complaints and close the loop with the reporting physician
- [ ] Establish an event-triggered review protocol so that any physician quality signal automatically generates a review — not a question about whether to file an incident report
