# Getting Started with Speedboat

[Home](../index.md) | [Docs](../docs/index.md) | [Guides](index.md) | [Ceremonies](ceremonies/index.md) | [Templates](../templates/index.md) | [Setup](../setup/index.md)

This guide is for a team trying Speedboat next week.

Every week, the boat chooses what to Land, limits what it starts, makes Run visible, and learns from what actually happened.

You do not need to understand the whole framework before starting.

There are two ways to use this guide:

- **Start this week:** follow only the Week 1 path below.
- **When the simple version stops being enough:** use [When To Add More Structure](when-to-add-more-structure.html).

**Recommended first read:** [One-Page Summary](../docs/one-page-summary.md)

---

## Start This Week

If you are trying Speedboat next week, do these things first and ignore the rest until Friday:

- Make sure the boat is small enough to move quickly. Speedboat works best with about 4-5 engineers.
- Reuse or create one board.
- Make active work visible as **Preview**, **Build**, or **Run** using swimlanes, labels, or another clear categorisation on the board.
- Keep your normal execution columns such as **To Do / In Progress / Done**.
- Pick 1-2 intended Landings for the week.
- Limit Preview and Build to 3 active items each.
- Run Monday Set Course, Wednesday Course Check, and Friday Landing.
- Create a [Landing Log](../templates/landing-log.md) on Friday.

---

## Core Concepts To Remember In Your First Week

If the team can answer these questions, you can start.

### 1. What counts as a Landing?

A Landing is meaningful work reaching its intended beneficiary. There are four types:

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

Keep at most 3 active Preview items and 3 active Build items.

If urgent Run breaks that limit, say so explicitly and name what is being paused. Hidden trade-offs are the problem, not the exception itself.

### 5. What do we do when something does not land this week?

We do not call the week a failure.

We say what did not land, why, and what happens next: continue, reduce scope, pause it, or replace it.

### 6. What belongs in Week 1 versus later?

Week 1 is for starting the rhythm, making work visible, and updating the Landing Log.

When you start to feel shaping pain, coordination pain, or reporting pain, use [When To Add More Structure](when-to-add-more-structure.html).

---

## Week 1 Action Checklist

This is the minimum viable rollout.

- [ ] Make sure the boat is small enough to move quickly, ideally about 4-5 engineers.
- [ ] Create or reuse one board.
- [ ] Make Preview, Build, and Run visible on the board using swimlanes, labels, or another clear categorisation.
- [ ] Keep normal Kanban execution columns such as To Do, In Progress, and Done.
- [ ] Move current in-flight work into the right lane. Do not wait for a clean start.
- [ ] Create one [Landing Log](../templates/landing-log.md).
- [ ] Pick 1-2 intended Landings for the week.
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

- [ ] **Monday:** Run [Set Course](ceremonies/set-course.md). Pick 1-2 intended Landings for the week.
- [ ] **Monday:** Check WIP. If you are above the limits, do not panic. Name what needs to finish before anything new starts.
- [ ] **Wednesday:** Run [Course Check](ceremonies/course-check.md). Ask what needs to change before Friday.
- [ ] **Friday:** Run [The Landing](ceremonies/the-landing.md). Record what landed, decide every active Preview, and update the Landing Log.
- [ ] **After Friday:** Resist the urge to retrospect on the process itself. You have one data point. The process will feel clunky. That's fine. Give it time.

### What "good" looks like in Week 1

- The team can name what lane their work is in
- WIP limits are visible, even if not yet respected perfectly
- At least one thing landed (any type)
- Every active Preview got a Friday decision
- The Landing Log reflects reality
- The board reflects reality

Give it time. Week 1 is about starting the habit, not proving the model.

---

## Week 2 and Beyond

- [ ] **Week 2:** If shaping is already painful, add [Route Planning](ceremonies/route-planning.md). If not, add it within the first few cycles.
- [ ] **Weeks 2–3:** Tune. Adjust ceremony timing if needed. Fix confusion about which lane work belongs in. Watch for zombie Previews.
- [ ] **Week 3-4:** If the team needs more structure, use [When To Add More Structure](when-to-add-more-structure.html).

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