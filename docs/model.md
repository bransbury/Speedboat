# Speedboat: The Operating Model

## Why now

Scrum was designed for a world where writing the code was the expensive part. That world has changed.

AI now materially accelerates how quickly we can understand unfamiliar systems, generate implementation options, build prototypes, refactor, write tests, explore edge cases, and produce demo-ready versions of future functionality. The bottleneck is no longer "how quickly can we write the code?"

It's increasingly:

- Are we building the right thing?
- Are we focused on the right work?
- Are we finishing what matters?
- Are we getting value in front of customers quickly?
- Are we learning fast enough?
- Are we keeping production safe and maintainable?

Faster code generation alone does not guarantee faster customer impact. Without a better operating model, AI can create the opposite: more half-finished work, more prototypes, more branches, more demos, more context switching, and more operational drag.

The cost of starting has collapsed. The cost of finishing (judgement, integration, review, rollout, support, learning) has not. That asymmetry is exactly what Speedboat is built to manage.

--- 

## The shift

Speedboat isn't about going faster. It's about starting less, learning faster, building fewer things at once, and landing more meaningful outcomes.

The core question changes:

| FROM | TO |
|---|---|
| What tickets are we committing to this sprint? | What meaningful thing are we landing this week, and what do we need to learn or finish to make that happen? |

And the cultural shifts behind it:

| FROM | TO |
|---|---|
| How much work can we start? | What meaningful thing can we land? |
| Is the ticket done? | Who benefited, what changed, what did we learn? |
| Product writes ideas, Engineering builds them. | Product and Engineering use fast Previews to learn together before committing deeply. |
| AI helps us produce more code. | AI helps us learn faster, focus better, and land value sooner. |

---

## Team size

A speedboat has few seats by design. The model works best with small teams of 4–5 engineers, where everyone has context, WIP limits feel natural rather than imposed, and the Friday Landing is a genuine conversation rather than a status parade.

Larger groups should split into multiple speedboats rather than scaling ceremonies up. Each boat has its own board, its own rhythm, and its own Landings. Coordination between boats happens at Route Planning, not daily.

---

## How AI changes the mechanics

AI doesn't just make Speedboat possible. It changes how work moves through the lanes:

- **Previews compress dramatically.** A Discovery Preview that would have taken a week of spike work can reach a decision point in 1–2 days with AI-assisted prototyping, code exploration, and rapid option generation.
- **Build benefits from faster implementation, but the quality gate stays the same.** AI accelerates writing code and tests. It does not accelerate judgement about what to build, how to roll it out safely, or whether it actually solves the customer problem.
- **Run becomes more proactive.** AI tooling makes it faster to investigate incidents, trace root causes, and generate fixes. This shifts the balance from reactive firefighting toward proactive improvement.
- **Route Planning gets sharper.** When the team can prototype cheaply, more ideas can go through Preview before committing to Build. Fewer wrong bets reach production.

The operating model creates the structure. AI provides the acceleration within it.

---

## The model

Speedboat uses three work lanes: Preview, Build, and Run.

Land is different. It is not a planning lane where work sits. It is the moment meaningful work reaches its intended beneficiary, and the outcome we log each week.

**Preview / Build / Run -> Landing**

### Preview

Quick prototypes, PoCs, or early demos that turn ideas into something tangible.

- Two flavours: **Discovery** (should we build this?) and **Demo** (make it real for Sales/customer conversations).
- Max 3 active. Timeboxed 1–5 working days.
- Every active Preview gets a decision at Friday's Landing: kill, park, continue, promote.

### Build

Production-grade work: turning validated or committed ideas into capability that ships.

- Max 3 active items at any time.
- Quality bar is unchanged: tests, security, observability, rollout, support impact.
- Sources: promoted Previews, committed roadmap, customer needs, platform necessities.
- Once a Build item starts, new requests become the next Preview or the next Build. They don't expand the current one.

### Landings

Landings are the heart of Speedboat: meaningful outcomes reaching their intended beneficiary.

- **Customer Landing:** feature live, beta, performance fix, real impact.
- **Business Landing:** Sales demo ready, customer conversation supported, GTM enabled.
- **Platform Landing:** debt removed, observability added, incident risk reduced.
- **Decision Landing:** a Preview killed, parked, or promoted with clear rationale.
- Every Landing must have a beneficiary, an outcome, and a reason it matters.

### How to interpret Landings

Not all Landings mean the same thing.

- **Customer Landings** show delivered value.
- **Business Landings** show commercial enablement.
- **Platform Landings** show capability and resilience.
- **Decision Landings** show learning and avoided waste.

A healthy team may produce all four. The important distinction is not to confuse learning or enablement with customer impact.

### Run

The honest, visible stream of operational work that keeps the business healthy.

- **Reactive Run:** incidents, urgent bugs, escalations, emergencies.
- **Proactive Run:** tech debt, dependency upgrades, observability, automation, performance.
- Target ~20% or less of capacity, but track the actual number honestly.
- Repeated reactive work should generate proactive improvement work.
- Proactive Run can count as a Landing when it creates a meaningful outcome, for example by reducing risk, improving reliability, or making future delivery easier.

---

## The weekly rhythm

Four light-touch checkpoints replace daily standups and two-week sprint planning.

The default rhythm is Monday / Wednesday / Friday, but teams should shift the cadence to match their working week. The important pattern is start-of-week steering, mid-week course correction, and end-of-week Landing.

| Ceremony | Duration | Purpose |
|---|---|---|
| Monday: Set Course | 30 min | Where are we going this week? Choose the intended Landing, confirm WIP, set ownership. |
| Wednesday: Course Check | 15 min | Are we still on track? Surface blockers and create permission to course-correct before the week is lost. |
| Friday: The Landing | 30 min | What landed, who benefited, what did we learn, and what decisions does each active Preview need? |
| Fortnightly: Route Planning | 60 min | Shape the route ahead: upcoming work, what needs Preview before Build, risks, and slicing into landings. |

---

## Decision rights

| Decision | Default owner |
|---|---|
| Intended Landing for the week | Product and Engineering together |
| Preview decision: kill / park / continue / promote | Product and Engineering together |
| Production readiness for Build | Engineering |
| Priority of what enters Preview or Build | Product |
| Run prioritisation during incidents | Engineering |

When Product and Engineering disagree, escalate quickly through the team's normal leadership path rather than leaving work in limbo.

---

## Two rules

### Landing mix

Over any 4-week window we expect at least some Customer or Business Landings, unless the team has explicitly chosen a Platform/Run-heavy period. Platform-heavy by accident is a signal to course-correct.

### Exception protocol

WIP limits are a steering rule, not a wall. Urgent Run, customer escalations, and leadership overrides are allowed, but the team names what is being paused to make room during the next Set Course or Course Check. Urgent Run does not violate Speedboat; hiding it does.

---

## What Speedboat is not

This matters as much as what it is.

**Not "move fast and break things."**
Preview can be rough because it's for learning. Build and Land must meet production standards.

**Not one-week Scrum.**
It's a steering rhythm for continuous flow, not a sprint commitment under a different name.

**Not "ship every Friday or fail."**
A Landing can be customer, business, platform, or decision-oriented. The ask is meaningful, not a forced release.

**Not a replacement for product strategy.**
Speedboat is the delivery operating system. Roadmap, customer judgement, and commercial context still matter.

---

## Principles

1. Customer impact is the unit of progress.
2. Start less work than we think we can.
3. Preview cheaply, decide quickly.
4. Build fewer things at once.
5. Prioritise Landing over starting.
6. Make Run work visible.
7. Use AI aggressively, but keep human ownership.
8. Product owns value; Engineering owns production readiness.
9. In short weeks, reduce scope, not discipline.