# UA5 — Stage 2 Analysis

The Stage 2 deliverable. Pulls together what exists in the space, who has a stake in the system beyond the users, who actually uses it, and what users are doing today when they need what the system would provide.

The sections are written in the order a reader would want to encounter them, but the student does not work on them in that order. Activities inform each other.

The positioning statement is revisited throughout. If any analysis contradicts a clause, the student revises `ua2-positioning-statement.md` — Stage 2 is the second pressure test on the statement.

---

## Landscape

A short survey of the space the system enters. Two or three pages of notes is usually enough.

### Adjacent products

- **Google Tasks / Trello-style checklist apps (incl. Todoist, Notion)** — solid at basic task capture (add a task, check it off), but completing a task doesn't clear it from view in any way that reads as progress. It just sits there checked off. Stev separately described this category as "ugly and hard to use" — same root problem showing up as a second symptom: nothing about these apps is attractive enough to be engaging. Overlaps with our project on capture; leaves a gap on making completion feel like visible momentum.
- **ChatGPT-generated to-do lists** — good at producing a reasonable task breakdown on request, but has no persistence or completion tracking at all. Every session starts from zero — the user has to re-describe and regenerate the list each time, even if a previous breakdown was already good. Overlaps on generating structure; leaves a gap on any kind of ongoing state.
- **Canvas (school LMS)** — low-maintenance in one specific way: the school posts everything (deadlines, assignments) for you, so there's no manual entry. But it only reflects the official due dates, not the student's own progress — there's no way to mark something personally complete ahead of the due date. Across multiple classes, that leads to confusion about what's actually still outstanding, hard-to-organize overlap, and its own motivation loss (nothing in it shows *your* progress, only the school's schedule).
- **Epic Todo List** — turns tasks into RPG-style quests (XP, gold, leveling). Overlaps directly on making completion feel rewarding; tonally leans fantasy-game/kid-oriented, not the direction OnTrack wants.
- **Duolingo** — streak/XP mechanic, mascot-driven tone. This is the direct reference point for the novelty-decay finding from Interview 3 (tanman) — the reward loop itself is the thing that eventually gets boring. Tonally playful/cartoonish, not the direction OnTrack wants.
- **Zombies, Run!** — narrative/mission framing turns a mundane activity (running) into a story to sustain motivation. Overlaps on using framing to make routine work feel less like a chore; tonally entertainment-first rather than something a student would want open next to actual schoolwork.

**Tonal takeaway:** OnTrack wants the engagement mechanic these three use, without the kid-game/mascot/fantasy tone — something that reads as mature and serious enough to sit next to real schoolwork, not as a toy.

### Open-source candidates

- None identified yet — Epic Todo List, Duolingo, and Zombies, Run! are all closed commercial products, not open-source. No open-source project has been looked at yet. Flagged below in "Open from this stage" as something to check before Stage 3.

### Category

- The category customers think they're shopping in: **planner**.
- What that category brings with it: expectation of **free** (traces directly to Stev — he said he'd only keep using a tool if it were easy to use and free) and **organized** as the baseline. "Feature-heavy" was the student's own instinct rather than something an interview said, and it initially sat in tension with "free" — free categories tend to stay simple, feature-heavy ones tend to charge.
- Resolution: **freemium**. Core stays free, simple, and organized — nothing load-bearing sits behind a paywall, so a normal user never feels money-locked. Deeper/more specific features are an optional paid tier for people who want to go further. This is a fit with the category's free expectation, not a fight against it.

### Inherited conventions

Conventions the project is taking on whether it knows it or not. For each, decide explicitly: keep, break on purpose, or note as open.

- Due dates — **keep**. Matches the evidence directly; the whole need is organized around deadlines.
- Checkboxes to mark a task done — **keep the interaction, break the aftermath**. Users expect to tap something to mark done, so the interaction stays. What breaks on purpose is what happens next — the "checked-off task just sits there, unchanged" convention from Google Tasks/Trello, which is the specific gap OnTrack exists to fill.
- Calendar view — **keep**. All three interviewees already think in calendar terms; fighting that mental model would cost more than it's worth.
- Multiple views to user preference (list, calendar, etc.) — **open**. A reasonable differentiator, but not something any interview actually asked for yet — don't treat it as confirmed need.

---

## Stakeholders and users

### Stakeholders

Everyone with a stake in whether the system succeeds beyond the users. Most stakeholders are not users. Most requirements come from stakeholders, not users.

| Stakeholder | Stake | Their version of "success" |
|---|---|---|
| [name or role] | [what they care about] | [what would make this stakeholder happy] |
| [name or role] | … | … |

For client-path projects: explicitly name the distinction between the client (stakeholder) and the people the client serves (users). Even when the client is enthusiastic about the user's needs.

- **Client:** [who]
- **Users the client serves:** [who]
- **Where their interests align:** [list]
- **Where their interests diverge:** [list — these are the friction points]

### Users (recap from Stage 1, with Stage 2 updates)

The user picture from Stage 1 with any updates Stage 2 work surfaced.

- **Primary user type:** [who]
- **Secondary user types (if any):** [who]
- **What's been added or revised since Stage 1:** [bullet list]

### Compliance and accessibility considerations

What has been surfaced about FERPA, COPPA, HIPAA, PII, accessibility, or any other regulatory / safety constraint relevant to the project. Capture in plain language; the student is not producing a compliance document.

- [constraint] — [how it applies; how the project will handle it]

---

## Jobs-to-be-done and scenarios

One subsection per job. Each has the four-question structure plus at least one scenario.

### Job 1 — [short title]

- **JTBD statement:** When I'm [situation], I want to [motivation], so I can [outcome].
- **How do we know it's a real job:** [specific evidence from Stage 1. A quote, an observation, a workaround witnessed firsthand.]
- **What people do today:** [step by step description of the current alternative. Not "they use a spreadsheet" — what columns, which sheet, what they do when the data doesn't fit.]
- **Why has the current way persisted:** [what it does well, what users would lose by switching. Chesterton's fence territory.]

#### Scenario 1.1 — [short title]

A narrative. The user starts with "I have this need" and ends with "my need is met." Includes at least one branch where something doesn't work the first time.

> [User] is doing [activity]. They need to [need]. They open [system / current alternative] and [first step]. Then [second step]. **Something goes wrong:** [thing]. They [recovery action]. Eventually [need is met or not].

**Reads back against positioning statement:** Does this story actually deliver the **key benefit** named in `ua2-positioning-statement.md`? [yes / no, with note]

#### Scenario 1.2 — [optional second scenario for the same job]

> [Narrative]

### Job 2 — [short title]

- **JTBD statement:**
- **How do we know it's a real job:**
- **What people do today:**
- **Why has the current way persisted:**

#### Scenario 2.1 — [short title]

> [Narrative]

---

## Open from this stage

Things flagged during Stage 2 that don't yet have a home — for the student to revisit later or carry into Stage 3.

- No open-source project has actually been looked at yet — worth a real search before Stage 3, since one might reveal conventions or a starting point worth using.
- Partner-suggested extension idea: a self-imposed website blocker (user blocks their own distracting sites, no other party involved). Maps directly onto tanman's finding (distraction from unrelated activity, not tool boredom) — worth formalizing as a job in Section 3 with that evidence attached, rather than designing it now.
- Canvas auto-carryover idea: a connection/integration so assignments posted on Canvas could flow into OnTrack automatically instead of manual entry. Not really a "convention" so much as a feature idea — worth exploring in Stage 3, since Canvas is already something tanman relies on and manual re-entry is exactly the kind of friction that kills follow-through.
