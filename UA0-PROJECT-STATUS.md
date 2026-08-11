# UA0 — Project Status

This file is maintained by the AI agents working with the student. The student does not edit it.

It records where the project is in the UA Framework process so any agent invocation can orient itself without re-reading every other document. It is updated at every meaningful checkpoint: the end of each pass in Stage 1, the end of each section in Stage 2, after each activity in Stage 3, and at every stage transition.

---

## Project header

- **Project name:** Gamified Productivity App
- **Path:** self-idea
- **Started:** 2026-06-22

## Current stage

Stage 3 — Specification

## Current pass or activity

Activity 1 — Screen inventory (`ua6-specification.md`)

## Positioning statement status

One line per clause. Status values: `not started` | `drafted from belief` | `drafted-unconfirmed` | `refined by research` | `evidenced by interview` | `stable`.

- Target customer: evidenced by interview
- Need or opportunity: evidenced by interview
- Product name: stable
- Product category: evidenced by interview
- Key benefit: evidenced by interview
- Primary competitive alternative: evidenced by interview
- Primary differentiation: evidenced by interview

## Completed checkpoints

A running list. Each entry is a single line: what was completed, and the date.

- Pass 1 — First draft, all seven clauses drafted from belief
- Interview 1 (Stev) — evidenced Target customer, Need or opportunity, Key benefit, Primary competitive alternative, Primary differentiation
- Interview 2 (null, 2026-08-03) — confirmed Need or opportunity, expanded Primary competitive alternative (AI-generated task lists), complicated and revised Key benefit and Primary differentiation (reward mechanics decay in engagement over time; visible structure is the durable core, not the reward skin)
- Interview 3 (tanman, 2026-08-04) — complicated Need or opportunity (drop-off can be salience/interruption, not just engagement — broadened basis for belief), expanded Primary competitive alternative (Canvas/school LMS), independently reconfirmed the novelty-decay finding behind Key benefit and Primary differentiation (kept at "evidenced by interview", not yet "stable" — one more confirming interview would make that call easy)
- Product name and Product category addressed (2026-08-06) — name changed from placeholder StudySprint/WorkSprinter to OnTrack (marked stable, internal decision); category changed from "gamified academic task planner" to "organized, engaging assignment tracker," demoting gamification to a supporting feature per the novelty-decay evidence from Interviews 2–3.
- **Stage 1 — Discovery complete (2026-08-06).** All seven positioning-statement clauses are "evidenced by interview" or "stable"; none remain "drafted from belief" or "drafted-unconfirmed". Verified against `ua2-positioning-statement.md` directly by the orchestrator before advancing.
- Stage 2, Section 1 — Landscape (2026-08-06): adjacent products (Google Tasks/Trello/Todoist/Notion, ChatGPT lists, Canvas, plus tonal references Epic Todo List/Duolingo/Zombies Run), category (planner, freemium resolution to the free-vs-feature-heavy tension), and inherited conventions (checkboxes kept, "checked task just sits there" broken on purpose, calendar view kept) are filled in. No open-source candidate identified yet — flagged as an open item. Two feature ideas surfaced (self-imposed website blocker, Canvas auto-carryover) and deferred to Section 3 / Stage 3 rather than designed now.
- Stage 2, Section 2 — Stakeholders and users (2026-08-09): stakeholders table (teacher, parent, school) filled in; client/user distinction marked N/A (self-idea path). User recap confirms one primary type, no secondary segment. Compliance pass surfaced PII/token handling for the deferred Canvas feature, accessibility commitments (screen readers, colorblind-friendly design, reduced-motion/no-flashing-lights mode, low-end device performance), FERPA and COPPA both noted as low-risk for now.
- Mid-Stage-2 positioning statement revision (2026-08-09): Job 2 in Section 3 (avoiding distraction, evidenced by tanman + a partner-suggested website-blocker idea) didn't cleanly fit the Key benefit clause as written. Key benefit broadened to add distraction-removal as an explicit secondary piece, deliberately kept behind "visible progress" in the sentence to reflect that it's single-sourced and not yet feature-tested, unlike the three-interview-deep visible-progress finding. Primary differentiation left unchanged — stays focused purely on visible progress.
- Stage 2, Section 3 — Jobs-to-be-done and scenarios (2026-08-10): Job 1 (organizing a heavy assignment load, evidenced by Stev and tanman) and Job 2 (avoiding distraction, evidenced by tanman) each have a scenario with a "something goes wrong" branch, read back against the positioning statement. A third job (Canvas auto-carryover) was considered but judged unnecessary for coverage — noted as available for Stage 3 if needed. **All three sections of `ua5-stage-2-analysis.md` are now filled in.**
- **Stage 2 — Analysis complete (2026-08-10).** Verified directly by the orchestrator: all three sections filled in (client/user distinction correctly marked N/A for self-idea path), positioning statement revisited and revised where Section 3 analysis contradicted it, both scenarios have a "goes wrong" branch, compliance/accessibility surfaced and answered. Two stale cross-references in `ua5-stage-2-analysis.md` (an unresolved-looking note that had actually been resolved, a "still to formalize" note for a job that was already built) corrected for consistency before advancing.

## Known gaps

Things the student and agent have flagged as not yet addressed. Carried forward across sessions until resolved or explicitly dropped.

- No interview has yet asked "anyone else worth talking to?" of Stev, null, or tanman — referral recruiting not yet attempted
- Falsification commitments for Interviews 1–2 were reconstructed after the fact rather than written in advance (see process note in `ua4-interview-plan.md`); Interview 3 onward writes commitments first — done for Interview 3

## Last updated

- **Date:** 2026-08-10
- **By:** ua-orchestrator 