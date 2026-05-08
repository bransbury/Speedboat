# Speedboat: The Operating Model

## Why now

Scrum was designed for a world where writing the code was the expensive part. That world has changed.

AI now materially accelerates how quickly we can understand unfamiliar systems, generate implementation options, build prototypes, refactor, write tests, explore edge cases, and produce demo-ready versions of future functionality. The bottleneck is no longer "how quickly can we write the code?"

AI makes you faster at building the wrong thing, too.

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

Acceleration is easy. Direction is hard.

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

Larger groups should split into multiple speedboats rather than scaling ceremonies up. Each boat has its own board, its own rhythm, and its own Landings. Coordination between boats should happen through a lightweight Fleet Sync rather than by scaling the boat-level ceremonies.

---

## Roles

Speedboat uses lightweight roles, not a heavyweight process structure.

- **Product Lead:** owns product priority, intended outcomes, and what enters Preview or Build.
- **Captain:** the engineering lead for the boat. Owns the health of the boat, WIP discipline, escalation, and engineering coordination.
- **Crew:** everyone contributes across Preview, Build, Run, and rotating facilitation.

The Captain is not a Scrum Master and does not own the backlog. Facilitation rotates, but accountability for the health of the boat does not.

---

## How AI changes the mechanics

AI doesn't just make Speedboat possible. It changes how work moves through the lanes:

- **Previews compress dramatically.** A Discovery Preview that would have taken a week of spike work can reach a decision point in 1–2 days with AI-assisted prototyping, code exploration, and rapid option generation.
- **Build benefits from faster implementation, but the quality gate stays the same.** AI accelerates writing code and tests. It does not accelerate judgement about what to build, how to roll it out safely, or whether it actually solves the customer problem.
- **Run becomes more proactive.** AI tooling makes it faster to investigate incidents, trace root causes, and generate fixes. This shifts the balance from reactive firefighting toward proactive improvement.
- **Route Planning gets sharper.** When the team can prototype cheaply, more ideas can go through Preview before committing to Build. Fewer wrong bets reach production.

The operating model creates the structure. AI provides the acceleration within it.

If you are using autonomous or semi-autonomous AI agents, the same rule still applies: they can accelerate exploration, implementation, and triage, but they do not reduce the finishing cost. Review, integration, rollout, and judgement remain human work. See [AI Agents in Speedboat](ai-agents.md).

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
- Big bets can span multiple weeks, but they should move through a sequence of meaningful partial Landings rather than staying as one invisible block of Build work.

### Big bets and multi-week Build

Some work will take 6–8 weeks. That is normal.

Speedboat does not require big bets to finish in a week. It does require them to stay visible, steerable, and sliceable.

Treat a big bet as a multi-week initiative with one umbrella outcome, but shape the active work into the next meaningful partial Landings.

Examples of partial Landings:

- API live behind a feature flag
- internal beta ready
- first customer cohort enabled
- observability and rollback path in place
- risky dependency removed

These are real Landings if they reach an intended beneficiary or materially reduce risk, enable downstream work, or make the next slice possible.

If a Build effort runs for more than 2 weeks without a meaningful partial Landing, Route Planning should re-slice it or name explicitly why no such Landing is currently possible.

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

Three core ceremonies a week. Zero status updates.

Four light-touch checkpoints replace daily standups and two-week sprint planning.

AI accelerates mistakes as efficiently as it accelerates progress. That is why the steering loop has to get shorter.

The default rhythm is Monday / Wednesday / Friday, but teams should shift the cadence to match their working week. The important pattern is start-of-week steering, mid-week course correction, and end-of-week Landing.

| Ceremony | Duration | Purpose |
|---|---|---|
| Monday: Set Course | 30 min | Where are we going this week? Choose the intended Landing, confirm WIP, set ownership. |
| Wednesday: Course Check | 15 min | Are we still on track? Surface blockers and create permission to course-correct before the week is lost. |
| Friday: The Landing | 30 min | What landed, who benefited, what did we learn, and what decisions does each active Preview need? |
| Fortnightly: Route Planning | 60 min | Shape the route ahead: upcoming work, what needs Preview before Build, risks, and slicing into landings. |
| Every 4 weeks: Learning Review | 30 min | Step back from the week-to-week flow. What is the work teaching us about WIP, Landing mix, Run load, and how the model is working? |

For teams running multiple boats, add one extra coordination point:

| Ceremony | Duration | Purpose |
|---|---|---|
| Fortnightly: Fleet Sync | 30 min | Surface cross-boat dependencies, align on shared platform priorities, and flag risks affecting multiple boats. |

Fleet Sync is not another planning layer and not a status meeting. It exists only for work that crosses boat boundaries.

The weekly learning slot in Friday's Landing is tactical: what changed this week and what should we adjust next week? The Learning Review is the slower feedback loop for the operating model itself.

Before the Learning Review, prepare a lightweight monthly stakeholder summary from the Landing Log and the last 4 Weekly Snapshots. It should answer three questions: what landed in the last 4 weeks, what the landing mix is telling you, and what is likely coming next.

---

## Multi-boat coordination

Fleet Sync is optional for a single boat and useful for environments running multiple boats.

- **Attendees:** one representative per boat, usually the Captain, plus product and engineering leadership.
- **Purpose:** surface dependencies before they become blockers, align on shared platform demand, and make cross-boat risks visible.
- **Outputs:** named dependency owners, explicit shared-priority decisions, and visible risks with an owner and next step.

Ownership stays lightweight:

- The boat needing a dependency owns making the need explicit.
- The boat providing the dependency owns committing or declining with a realistic timing view.
- Engineering leadership breaks ties when multiple boats need the same shared platform capability.
- Product leadership joins the decision when the trade-off affects customer or business outcomes across boats.

Use Fleet Sync to expose cross-boat issues early. Do not turn it into a second Route Planning session.

---

## Intake flow

New work enters Speedboat through an **unshaped backlog**.

This is where customer feedback, Sales requests, engineering observations, roadmap items, leadership asks, and other new ideas go before the team decides whether they should become Preview, Build, or Run.

Keep the flow simple:

- **Unshaped backlog:** new ideas and requests waiting for triage.
- **Shaped queue:** work reviewed in Route Planning and tagged as needs Preview, ready for Build, or blocked.
- **In flight:** work actively in Preview, Build, or Run.

Between Route Planning sessions, the Product Lead and Captain triage incoming work against current WIP and current commitments.

- If it is urgent, use Run or the exception protocol and name what gets paused.
- If it is important but not urgent, add it to the unshaped backlog.
- If it creates a cross-boat dependency or risk, surface it in Fleet Sync.

Only Route Planning should promote non-urgent work from the unshaped backlog into the shaped queue.

Do not quietly inject unshaped work into Build mid-week. New work becomes visible when it enters the system, not when it surprises the team.

---

## Decision rights

| Decision | Default owner |
|---|---|
| Intended Landing for the week | Product Lead and Captain together |
| Preview decision: kill / park / continue / promote | Product Lead and Captain together |
| Production readiness for Build | Captain / Engineering |
| Priority of what enters Preview or Build | Product Lead |
| Run prioritisation during incidents | Captain |

When Product Lead and Captain disagree, they should resolve it explicitly and quickly. If they cannot resolve it within the same working day, the Captain initiates escalation to the next product and engineering leaders rather than leaving work in limbo.

---

## Two rules

### Landing mix

Over any 4-week window we expect at least some Customer or Business Landings, unless the team has explicitly chosen a Platform/Run-heavy period. Platform-heavy by accident is a signal to course-correct.

### Exception protocol

WIP limits are a steering rule, not a wall. Urgent Run, customer escalations, and leadership overrides are allowed, but the team names what is being paused to make room during the next Set Course or Course Check. The Captain owns enforcing this exception protocol. Urgent Run does not violate Speedboat; hiding it does.

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