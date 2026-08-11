# UA6 — Specification

The Stage 3 deliverable. Pulls everything from Stages 1 and 2 into a single document that a developer — human or AI — can build from.

The screens are the spine. In a small project the screens are the functional requirements: each screen names what the system does in terms a user would recognize.

MVP scoping is not a section in this document. Which screens get built first emerges during wireframing as the deadline forces choices, not from a planning artifact written before the work begins.

---

## Overview

### Positioning statement

> For a high school student who wants to stay on top of schoolwork but struggles to turn assignments into consistent follow-through,
> the OnTrack is an organized, engaging assignment tracker
> that turns deadlines, study routines, and assignment progress into visible progress you can act on right now — the structure carries it, not the streak — with tools to remove the distractions most likely to pull you off track.
> Unlike generic to-do apps, static planners, or AI-generated task lists,
> our product keeps a live, visible picture of a student's progress — what's due, what's next, how far they've gotten — with streaks and rewards as an on-ramp, not the thing holding it together long-term.

### Summary

[To be written by the student.]

---

## Screen inventory

A flat list of every screen the system needs.

| # | Screen | Purpose (one sentence) | Scenarios that pass through it |
|---|--------|------------------------|--------------------------------|
| 1 | Login (Google) | Let the student sign in with their Gmail account; also creates the account on first use. | Entry point — precedes both scenarios |
| 2 | 2-Step Verification | Confirm identity with a second factor after Google login. | Entry point — precedes both scenarios |
| 3 | Assignments (List / Board / Calendar views) | Show the student's assignment chunks and live, visible progress state — same data, three switchable views: a simple list, a board with columns arranged by due date and color-coded by assignment type, and a calendar. | 1.1 |
| 4 | Add Assignment | Let the student enter a new assignment, its due date, and its type (for the Board view's color-coded columns). | 1.1 |
| 5 | Assignments — Empty State | Show a new student (no assignments yet) how to get started. | Not from a scenario — standard state |
| 6 | Behind-Schedule Adjustment | Show the student what got missed and let them redistribute it across remaining days. | 1.1 (the "goes wrong" branch) |
| 7 | Focus Mode Setup | Let the student choose which sites to block and for how long. | 2.1 |
| 8 | Focus Mode Active | Show the running block session (timer, blocked list) while it's in effect. | 2.1 |
| 9 | Blocked Site Intercept | Show up in place of a site the student tries to visit while it's blocked. | 2.1 (the "goes wrong" branch) |
| 10 | Focus Mode Complete | Confirm the session ended and let the student unblock manually if they want. | 2.1 |
| 11 | Settings | House accessibility options (colorblind-friendly mode, reduced-motion/no-flashing mode) and account settings. | Not from a scenario — standard screen |
| 12 | Error state | Shown when something that touches the network fails (login, saving an assignment). | Not from a scenario — standard state |

Includes screens not surfaced by any scenario, named explicitly so they don't surprise the student during wireframing:

- Login / authentication — **included** (Google login doubles as account creation on first use, so no separate signup screen)
- Settings — **included**
- Empty state — **included** (Home — Empty State)
- Error state — **included**
- Confirmation / success states for irreversible actions — **none yet**; nothing in the current scope deletes or irreversibly changes something. Revisit if that changes.

When the same screen appears in multiple scenarios, it's one entry. Those screens are load-bearing and deserve extra care.

---

## Screen descriptions

One subsection per screen. All five parts required.

### [Screen 1 — name]

- **Purpose:** [one sentence]
- **Who lands here:** [user type and how they got here — clicked X, redirected from Y, opened the bookmarked URL]
- **What's shown:** [data and content that appears — not layout, content. What information does the user need to do what they came to do?]
- **What they can do:** [each action, named]
  - [action 1]
  - [action 2]
- **Where each action goes:**
  - [action 1] → [next screen | confirmation | state change | error]
  - [action 2] → [destination]

---

## Requirements

Things that matter for what gets built but don't live anywhere else in this document. Accessibility, performance, security, data handling. If a requirement is already implicit in a screen description, it does not need to be repeated here. Short — usually a handful of bullets.

- [requirement]

---

## Constraints and assumptions

What's fixed, what's being assumed, what's out of scope.

- [constraint or assumption]

---

## Open questions

Things deferred or unresolved that a developer building from this would need to know about.

- [question]
