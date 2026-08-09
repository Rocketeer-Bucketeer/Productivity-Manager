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
| Teacher | Never sees the app directly, but benefits if it works | More assignments turned in on time — a higher on-time submission rate across their students |
| Parent | Wants their child to do well in school and be organized about it | Enhanced academic and organizational performance from their child — better grades, less scrambling |
| School (as an institution) | Mostly redundant with the teacher row, but distinct in one way: aggregate student performance on state tests affects the school itself (ratings, funding, reputation) | Improved state test performance among students who use tools like OnTrack |

For client-path projects: explicitly name the distinction between the client (stakeholder) and the people the client serves (users). Even when the client is enthusiastic about the user's needs.

- **Client:** [who]
- **Users the client serves:** [who]
- **Where their interests align:** [list]
- **Where their interests diverge:** [list — these are the friction points]

### Users (recap from Stage 1, with Stage 2 updates)

The user picture from Stage 1 with any updates Stage 2 work surfaced.

- **Primary user type:** Motivated-but-inconsistent high school student (from Stage 1 positioning statement) — no separate segment needed; even distraction-heavy cases like tanman fold into this same type rather than forming their own.
- **Secondary user types (if any):** None identified.
- **What's been added or revised since Stage 1:**
  - Broadened understanding of *why* drop-off happens — not just low engagement (null) but salience/interruption from unrelated distractions (tanman). Same user type, two different failure modes.
  - The self-imposed website-blocker idea responds directly to the interruption/salience failure mode.

### Compliance and accessibility considerations

What has been surfaced about FERPA, COPPA, HIPAA, PII, accessibility, or any other regulatory / safety constraint relevant to the project. Capture in plain language; the student is not producing a compliance document.

- **PII / data handling:** The core app doesn't need to collect personal information — just assignments and due dates. The one exception is the (deferred) Canvas auto-carryover feature: if built, it requires the student to authorize access to their real Canvas account, meaning an access token tied to a real school account and assignment data pulled from a school system. Not urgent now since that feature is deferred to Stage 3, but flagged so it isn't treated as "no data handling needed" once it's actually built.
- **Accessibility (WCAG-adjacent):** Student has already identified several real considerations — screen reader support, colorblind-friendly design, and a reduced-motion / no-flashing-lights mode in case any future feature uses flashing effects (photosensitive seizure risk). Also raised device performance — the app shouldn't require a high-end computer to run, which is an equity concern as much as a technical one. None of these are designed yet; captured here as commitments to carry into Stage 3.
- **FERPA:** Not directly triggered by the core app (it's a personal student tool, not a school-run system holding official education records), but worth keeping in mind if the Canvas integration ships, since that touches data that originates from a school's system.
- **COPPA:** Unlikely to apply — target users are high schoolers, generally 14+, not under 13. Not flagged as an active concern, but noted in case an edge case (a younger student) comes up later.

---

## Jobs-to-be-done and scenarios

One subsection per job. Each has the four-question structure plus at least one scenario.

### Job 1 — Organizing a heavy assignment load

- **JTBD statement:** When I'm facing a heavy workload with assignments piling up, I want an easy way to organize and see what's next, so I can get through the overwhelming stretch without falling behind.
- **How do we know it's a real job:** Stev directly said the workload feels too large for the time available and the work itself is hard to do — an unprompted complaint. Tanman already does a manual version of this job: he checks his calendar to see how many days he has left, then splits the work across those days — a real, active behavior under exactly this situation.
- **What people do today:**
  - Stev: tracks in a planner or by memory, no described active splitting strategy.
  - Tanman: opens his calendar, counts the days available before the deadline, manually divides the work across them.
  - null: uses a calendar and asks ChatGPT to generate a task breakdown — but has to redo it from scratch every time, since nothing persists.
- **Why has the current way persisted:** Manual splitting (tanman) survives because it costs nothing — it's just a calendar he already has open. ChatGPT-list generation (null) survives because it's genuinely good at producing a reasonable breakdown on request, even without tracking. Both are "good enough to start with," which is exactly why nobody's switched away from them yet.

#### Scenario 1.1 — Recovering after a distraction wipes out a day

> A student opens OnTrack on Sunday night after realizing three assignments and a test are due across the coming week. They enter each assignment with its due date; OnTrack splits the work into daily chunks and shows a live, visible progress state. Monday and Tuesday go fine — they check off each day's chunk and watch the progress state move. **Something goes wrong:** midweek, they get pulled into a game for a few hours and forget to open the app entirely. By the time they remember, a full day's planned chunk is sitting untouched. They open OnTrack and immediately see the gap — the plan is visibly behind where it should be, not just quietly forgotten like it would be with a plain calendar. They redistribute the missed chunk across the remaining days and finish the last assignment the night before it's due.

**Reads back against positioning statement:** Mostly yes — the visible, live structure is what surfaces the gap and drives the recovery, not a streak. Worth being honest about a limit: this scenario shows the app helping *after* the student remembers to open it — it doesn't stop them from getting pulled into the game in the first place. That's exactly the hole the website-blocker idea would need to fill, which argues for taking that feature seriously in Stage 3 rather than treating it as a nice-to-have.

### Job 2 — Avoiding distraction while trying to focus

- **JTBD statement:** When I'm trying to focus on assignments, I want to keep myself from getting pulled into distracting sites or apps, so I can actually get the work done instead of drifting away.
- **How do we know it's a real job:** Tanman directly described this happening — "i was playing games and completely forgot about the project" — and his own recovery method was "makihng sure that no distractions [were] around me and focused on working." That's a self-identified need he already acts on manually. **Caveat:** this is currently single-sourced (tanman only); Stev and null didn't describe this specific coping behavior, so it shouldn't be treated as universally confirmed the way Job 1 is.
- **What people do today:** Tanman manually removes himself from distracting situations after the fact — pure self-discipline, no tool support, and only after he's already lost time to the distraction.
- **Why has the current way persisted:** It costs nothing and requires no new tool — it's just willpower. But it's inconsistent, which is exactly why he needed to "recover" in the first place rather than never losing the time at all.

#### Scenario 2.1 — Blocking the site before it becomes a problem

> A student sits down to start homework and knows from experience they'll end up on a game site if they're not careful. Before starting, they open OnTrack's focus mode and add the game site to a self-imposed block list for the next two hours. They start working. **Something goes wrong:** twenty minutes in, they get the urge to check the site anyway and try to open it — it's blocked, and instead of giving up, they get mildly annoyed but stay on the assignment since the path of least resistance is now just to keep working. They finish the two-hour block having made real progress, then unblock the site themselves afterward.

**Reads back against positioning statement:** Partial fit. The positioning statement's key benefit is about *visible progress*, not *distraction prevention* — this scenario delivers a real, evidenced need, but it's a different mechanism than what's currently written in the paragraph. Worth flagging rather than quietly stretching the key benefit to cover it: either this feature is a deliberate scope expansion beyond the current positioning statement, or it stays framed as a supporting feature that serves the same underlying "visible momentum" need from a different angle (removing what interrupts momentum, rather than showing momentum). Not resolved here — carried to "Open from this stage."

---

## Open from this stage

Things flagged during Stage 2 that don't yet have a home — for the student to revisit later or carry into Stage 3.

- No open-source project has actually been looked at yet — worth a real search before Stage 3, since one might reveal conventions or a starting point worth using.
- Partner-suggested extension idea: a self-imposed website blocker (user blocks their own distracting sites, no other party involved). Maps directly onto tanman's finding (distraction from unrelated activity, not tool boredom) — worth formalizing as a job in Section 3 with that evidence attached, rather than designing it now.
- Canvas auto-carryover idea: a connection/integration so assignments posted on Canvas could flow into OnTrack automatically instead of manual entry. Not really a "convention" so much as a feature idea — worth exploring in Stage 3, since Canvas is already something tanman relies on and manual re-entry is exactly the kind of friction that kills follow-through.
- Not yet addressed: whether a school's IT/policy stance would matter for the Canvas integration idea — e.g., whether a student can authorize their own Canvas API access without needing school approval. Worth checking before treating that feature as a given.
- The website-blocker job (Job 2) doesn't cleanly deliver the key benefit as currently written ("visible progress") — it's a distraction-prevention mechanism, not a progress-visibility one. Unresolved: is this a deliberate scope expansion of the positioning statement, or does it stay framed as a supporting feature serving the same underlying need from a different angle? Worth a real conversation with `positioning-statement` before Stage 3, not a quiet stretch of the existing wording.
