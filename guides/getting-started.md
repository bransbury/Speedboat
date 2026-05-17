# Getting Started with Speedboat

[Home](../index.md) | [Docs](../docs/index.md) | [Guides](index.md) | [Ceremonies](ceremonies/index.md) | [Templates](../templates/index.md) | [Setup](../setup/index.md)

This guide is for a team trying Speedboat next week.

Speedboat helps AI-accelerated teams finish meaningful work, not just start more work. In Week 1, the goal is simple: limit starts, make Run visible, and prove what Landed.

You do not need to understand the whole framework before starting.

There are two ways to use this guide:

- **Start next week:** follow only the Week 1 path below.
- **Add more structure later:** use [When To Add More Structure](when-to-add-more-structure.md) when the basic version stops being enough.

**Recommended first read:** [Speedboat on a Page](../docs/one-page-summary.md)

---

## Start This Week

If you are trying Speedboat next week, do only the basics first:

- Make active work visible as **Preview**, **Build**, or **Run** using swimlanes, labels, or another clear categorisation on the board.
- Keep your normal execution columns such as **To Do / In Progress / Done**.
- Pick **1–2 intended Landings** for the week.
- If that choice feels fuzzy, use [How to Choose This Week's Landing](choosing-what-to-land.md).
- Limit active work to **max 3 Preview** and **max 3 Build** items in flight.
- Run **Set Course** on Monday, **Course Check** on Wednesday, and **The Landing** on Friday.
- Create a [Landing Log](../templates/landing-log.md) before Friday and update it in The Landing.

You do not need to redesign Jira, clean the whole backlog, or introduce every template. Start the rhythm first.

---

## Core Concepts To Remember In Your First Week

If the team can answer these questions, you can start.

### 1. What counts as a Landing?

A Landing is a meaningful outcome: something reached a real beneficiary, or new evidence changed what happens next. There are four types:

- **Customer:** value live to a user or customer
- **Business:** a sales, GTM, or stakeholder outcome
- **Platform:** a resilience, debt, or capability improvement
- **Decision:** a meaningful Preview outcome, including kill, park, or promote

If something mattered to someone and changed what is true now, it can count as a Landing.

### 2. How do we classify work as Preview, Build, or Run?

- **Preview:** work to learn quickly before committing deeply
- **Build:** production-grade work we have decided to ship properly
- **Run:** operational work, both reactive and proactive

Use [Which Lane?](which-lane.md) whenever the team is unsure.

### 3. What are the three weekly ceremonies for?

- **Set Course:** choose the intended Landing for the week
- **Course Check:** decide what needs to change before the week is lost
- **The Landing:** record what landed, decide every active Preview, and capture learning

These are steering points, not status meetings.

### 4. What is the WIP rule?

Keep at most 3 active Preview items and 3 active Build items in flight.

A WIP item is not a subtask. It is a meaningful unit of work the team is steering: a prototype, a feature slice, a production change, or another outcome-sized piece of work.

If urgent Run breaks that limit, say so explicitly and name what is being paused. Hidden trade-offs are the problem, not the exception itself.

### 5. What do we do when something does not land this week?

We do not call the week a failure.

We say what did not land, why, and what happens next: continue, reduce scope, pause it, or replace it.

### 6. What belongs in Week 1 versus later?

Week 1 is for starting the rhythm, making work visible, and updating the Landing Log.

When you start to feel shaping pain, coordination pain, or reporting pain, use [When To Add More Structure](when-to-add-more-structure.md).

### 7. Who owns what?

- **Product Lead:** owns product priority and intended outcomes.
- **Captain:** the engineering lead for the boat, typically the tech lead, team lead, or engineering manager closest to the day-to-day work. Owns boat health, escalation, and WIP discipline.
- **Crew:** the rest of the engineering team. The Captain works with the crew, but carries explicit accountability for the health of the boat.

The facilitator may update the Landing Log live, but the Captain is accountable for making sure it stays current. Product Lead is not part of the crew, but should stay close to Landing and Preview decisions.

---

## Week 1 Action Checklist

This is the minimum viable rollout.

- [ ] Make sure the boat is small enough to move quickly, ideally about 4–5 engineers.
- [ ] Create or reuse one board.
- [ ] Make Preview, Build, and Run visible on the board using swimlanes, labels, or another clear categorisation.
- [ ] Keep normal Kanban execution columns such as To Do, In Progress, and Done.
- [ ] Move current in-flight work into the right lane. Do not wait for a clean start.
- [ ] Create one [Landing Log](../templates/landing-log.md).
- [ ] Pick 1–2 intended Landings for the week.
- [ ] Limit Preview and Build to 3 active items each.
- [ ] Run [Set Course](ceremonies/set-course.md), [Course Check](ceremonies/course-check.md), and [The Landing](ceremonies/the-landing.md).
- [ ] Update the Landing Log on Friday.

Week 1 should optimise for visibility, not tooling polish.

---

## Before You Start

Make sure you can answer these questions:

- **How long is the trial?** Four weeks is usually enough to get signal without dragging it out.
- **Does the team know this is coming?** Speedboat requires opt-in, not surprise.
- **Is Product aligned?** Product and Engineering need a shared view of Preview and Landing decisions.
- **What is your current WIP?** Count active items now so the team can see the change clearly.

---

## Week 1: Go

You are not trying to be perfect. You are trying to start the rhythm.

- [ ] **Monday:** Run [Set Course](ceremonies/set-course.md). Pick 1–2 intended Landings for the week.
- [ ] **Monday:** If priority is unclear, use [How to Choose This Week's Landing](choosing-what-to-land.md).
- [ ] **Monday:** Check WIP. If you are above the limits, do not panic. Name what needs to finish before anything new starts.
- [ ] **Wednesday:** Run [Course Check](ceremonies/course-check.md). Ask what needs to change before Friday.
- [ ] **Friday:** Run [The Landing](ceremonies/the-landing.md). Record what landed, decide every active Preview, and update the Landing Log.
- [ ] **After Friday:** Resist the urge to retrospect on the process itself. You have one data point. The process will feel clunky. That's fine. Give it time.

### What good enough looks like in Week 1

- The team can name what it tried to Land.
- Current work is visible as Preview, Build, or Run.
- Run work is no longer hidden.
- At least one outcome, decision, or learning is recorded.
- Every active Preview gets a Friday decision.
- The team knows what to adjust next week.

Give it time. Week 1 is about starting the habit, not proving the model.

---

## Week 2 and Beyond

- [ ] **Week 2:** If shaping is already painful, add [Route Planning](ceremonies/route-planning.md). If not, add it within the first few cycles.
- [ ] **Weeks 2–3:** Tune. Adjust ceremony timing if needed. Fix confusion about which lane work belongs in. Watch for zombie Previews.
- [ ] **Weeks 3–4:** If the team needs more structure, use [When To Add More Structure](when-to-add-more-structure.md).

If you continue after the trial, keep the Learning Review as the standing monthly feedback loop.

---

## Doing It Right

You are doing Speedboat right if the team has:

- fewer hidden commitments
- fewer half-finished threads
- clearer weekly outcomes
- a more honest view of operational load

You are not doing Speedboat right if:

- everything becomes a Landing
- Previews never end
- Run is hidden
- WIP limits are routinely ignored without being named
- Friday becomes a status meeting

---

## Common Week 1 Problems

- **WIP is way over the limit:** Do not force-stop work. Name the excess, finish what you can, and respect the limits for new starts.
- **Nobody landed anything:** That is fine for Week 1. Adjust ambition, not the model.
- **"I don't know which lane this is":** Use [Which Lane?](which-lane.md). If it is genuinely ambiguous, default to Preview.
- **A P1 incident blew up the week:** That is Run. Name what got paused.
- **The team thinks this is just one-week sprints:** Reinforce that the weekly cadence is for steering, not commitment.
- **Someone asks where the story points are:** Gone. Speedboat measures Landings, not estimates.

---

## You're Ready

The most important thing in Week 1 is not running the model perfectly. It's starting the rhythm and making work visible. Everything else can be tuned.

If you get stuck, check the [FAQ](../docs/faq.md). If something's missing from this repo, [open an issue](https://github.com/bransbury/Speedboat/issues).

Good luck. Start less. Learn faster. Land more.
