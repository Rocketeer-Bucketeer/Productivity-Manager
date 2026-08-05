# UA2 — Positioning Statement

The deliverable of Stage 1. Drafted in Pass 1 from current belief, revised across Passes 2–4 as research and interview evidence comes in. Every clause must be defensible by the time Stage 1 exits.

The statement at the top is the public-facing artifact — short, clean, one paragraph. The evidence record below it is the working document where the student's thinking lives. The messiness in the evidence record is the point. Cleaning it up to look polished destroys the record of learning. This is a living document; its git history is part of the deliverable.

---

## Statement

> For a high school student who wants to stay on top of schoolwork but struggles to turn assignments into consistent follow-through,
> the StudySprint is a gamified academic task planner
> that turns deadlines, study routines, and assignment progress into visible progress you can act on right now — the structure carries it, not the streak.
> Unlike generic to-do apps, static planners, or AI-generated task lists,
> our product keeps a live, visible picture of a student's progress — what's due, what's next, how far they've gotten — with streaks and rewards as an on-ramp, not the thing holding it together long-term.

---

## Status

Per-clause status. Mirrors the per-clause status in `UA0-PROJECT-STATUS.md`.

- **Target customer:** evidenced by interview
- **Need or opportunity:** evidenced by interview
- **Product name:** drafted from belief
- **Product category:** drafted from belief
- **Key benefit:** evidenced by interview
- **Primary competitive alternative:** evidenced by interview
- **Primary differentiation:** evidenced by interview

Status values: `not started` | `drafted from belief` | `drafted-unconfirmed` | `refined by research` | `evidenced by interview` | `stable`.

---

## Evidence

One subsection per clause. Updated continuously across all five passes.

### Target customer

- **Current belief:** High school student who is motivated academically, but who loses momentum when the workload becomes fragmented and the next step is not obvious.
- **Basis for the belief:** This is the right customer because the product is designed around school-specific execution: assignments, deadlines, and study routines that need visible follow-through.
- **Evidence found:**
  - Behaves like a self-directed student who wants to perform well but needs support making work feel actionable.
  - Likely values structure, accountability, and visible progress more than pure scheduling flexibility.
  - Interview 1 (Stev): currently tracks assignments in a planner or by memory, suggesting a low-friction, simple workflow is more important than a complex planning system.
  - Interview 2 (null): also fits the profile — motivated enough to use a calendar and an AI assistant to stay on top of work, but still loses the thread when the tool doesn't hold his attention.
- **Alternatives considered:**
  - A general productivity user who just wants a calendar or a task list.
  - A student who is not strongly motivated by streaks or game-like progress.
- **What would change my mind:**
  - If the user’s main pain is not follow-through but something like time management, test prep, or general life organization.

### Need or opportunity

- **Current belief:** College-bound students need a system that turns schoolwork into visible momentum instead of a passive checklist that gets ignored.
- **Basis for the belief:** The frustration is not only forgetting tasks — passive tools don't stay in view for two different reasons. Some people (null) find the tool itself unengaging and drift away. Others (tanman) get pulled into something unrelated and the tool isn't salient enough to interrupt that. "Visible momentum" needs to cover both — but that can't just mean notifications, since a nudge meant to pull someone back can just as easily read as naggy and get avoided instead.
- **Evidence found:**
  - The user’s problem appears to be follow-through consistency, not merely task capture.
  - The opportunity is strongest where motivation and structure need to reinforce each other.
  - Interview 1 (Stev): the workload feels too large for the time available and the work itself is hard to do, pointing to a need for momentum support rather than just reminders.
  - Interview 2 (null): gets easily distracted specifically because of the "non-engagement" of the calendar he uses — direct support for the idea that a passive checklist loses him, where something visible and current would not.
  - Interview 3 (tanman): drop-off wasn't tool-boredom — he was "playing games and completely forgot about the project." His calendar/Canvas method is otherwise structured. This points to a salience/interruption need, distinct from null's engagement need.
- **Alternatives considered:** Standard planners, paper calendars, generic to-do apps, and sticky-note systems.
- **What would change my mind:** If the user already reports that a planner or study-system reliably carries them through execution without extra motivation. Also: if a future interview shows that any kind of proactive nudge — notification-shaped or not — gets avoided/dismissed rather than acted on, "visible momentum" needs a different mechanism entirely for the tanman-type case.

### Product name

- **Current belief:** WorkSprinter
- **Basis for the belief:** The name signals both academic focus and momentum-building action, which fits a product centered on school tasks and streak-style progress.
- **Evidence found:**
- **Alternatives considered:** StudyQuest, GradeFlow, TaskStreak, ScholarLoop.
- **What would change my mind:** If a more descriptive or more brandable name better fits the product’s real interface and audience.

> Mostly internal; thin evidence here is acceptable.

### Product category

- **Current belief:** A gamified academic task planner.
- **Basis for the belief:** The product is primarily about helping students manage school tasks while making progress visible and motivating through a lightweight game-like loop.
- **Evidence found:**
  - The core workflow is task tracking, but it is centered on academic follow-through and momentum.
  - The key differentiator is not raw planning features alone, but progress encouragement tied to school execution.
- **Alternatives considered:** School planner, study app, productivity tracker, habit app.
- **What would change my mind:** If the app ends up focusing more on general life productivity than academic work.

### Key benefit

- **Current belief:** It turns assignments and academic routines into visible progress that's easy to act on right now — the structure carries it, not the streak.
- **Basis for the belief:** For a student who is motivated but inconsistent, visible progress lowers the barrier to taking the next step. Interview 2 showed that the reward/streak mechanic itself has a shelf life, so the benefit needs to rest on the visible structure, not on the reward loop staying novel forever.
- **Evidence found:**
  - The user is likely seeking a psychological lift as much as a planning tool.
  - A visible streak or reward loop can make execution more repeatable, at least at first.
  - Interview 1 (Stev): the student explicitly said visible progress, streaks, or rewards would help them stay consistent.
  - Interview 2 (null): said streaks/rewards would help "the first times" he used it, but would become boring and unengaging after a while — "like how people move on from a video game to another one." He clarified this isn't about refusing to rely on gamification in principle; it's that the mechanic itself predictably decays in engagement over time.
  - Interview 3 (tanman), independently and unprompted: about Duolingo, "overtime it get s boring but sometimes its fun. when i am learning smt new its gets very interesting." A second, separate person describing the same pattern — engagement tracks novelty of content, not the streak/reward mechanism itself.
- **Alternatives considered:** Better reminders, more detailed scheduling, stricter deadlines. Earlier belief — "makes follow-through feel easier to sustain" — dropped, since a mechanic that reliably goes stale can't be the thing that sustains anything.
- **What would change my mind:** If the real pain point is mostly organization rather than motivation. Also: if a future interview shows the novelty-decay problem doesn't apply once visible progress itself (not the reward skin) is what's hooking the user.

### Primary competitive alternative

- **Current belief:** Generic to-do apps and planners (Todoist, Notion, Google Tasks), AI tools used to generate task lists on demand, and school LMS platforms (Canvas) used to check remaining time.
- **Basis for the belief:** These already solve task capture, but none of them keep a live, visible state of progress — they show a list, not momentum.
- **Evidence found:**
  - Students already have access to general productivity tools, yet still struggle with follow-through.
  - The gap is likely in motivational reinforcement and academic context, not in raw planning capability.
  - Interview 1 (Stev): described existing apps as ugly and hard to use, and said they would only keep using a tool if it were easy to use and free.
  - Interview 2 (null): uses a calendar *and* asks ChatGPT to generate to-do lists — the alternative set is broader than plain to-do apps. He dislikes that the AI is "too servile": it complies with the request but adds no structure or accountability of its own.
  - Interview 3 (tanman): uses a calendar app and checks Canvas "to see how much time I have left" — the alternative set now includes school LMS platforms, not just consumer to-do apps and AI assistants.
- **Alternatives considered:** Paper planners, digital calendars, study timer apps, and classroom management tools.
- **What would change my mind:** If the user’s main competition is a more specialized academic planner rather than a general productivity tool or AI assistant.

### Primary differentiation

- **Current belief:** Our product keeps a live, visible picture of a student's progress — what's due, what's next, how far they've gotten — with streaks and rewards as an on-ramp, not the thing holding it together long-term.
- **Basis for the belief:** The target customer needs a system that shows real state, not just a list. The reward layer helps get them started, but Interview 2 showed the reward mechanic itself decays in engagement over time — so the visible structure has to be what carries it after the novelty wears off.
- **Evidence found:**
  - The user's challenge seems to sit at the intersection of planning and motivation.
  - Interview 1 (Stev): strongest product signals are simple usability, low cost, and visible progress/reward feedback.
  - Interview 2 (null): streaks/rewards help "the first times" but become boring after a while, "like how people move on from a video game to another one" — a mechanic that decays on a schedule can't be the primary moat.
  - Interview 2 (null): dislikes that AI to-do assistants are "too servile" — they comply but add no structure. Read together with the novelty-decay point, the moat looks like it's the structure itself, not any one motivational skin on top of it.
  - Interview 3 (tanman): independently described the same Duolingo novelty-decay pattern, unprompted. Two separate people now describe reward mechanics losing their pull over time — this is no longer a one-off from null.
- **Alternatives considered:** Earlier belief — "combines academic planning with streak-based motivation and progress rewards" as the primary differentiator — dropped in favor of visible structure as the core, with rewards as a supporting on-ramp. Also considered: reward systems in habit apps, school-management apps, gamified productivity tools generally.
- **What would change my mind:** If a future interview shows the reward loop itself — not the visible-state structure — is what actually retains users long-term, this should revert.
