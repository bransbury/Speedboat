# SPEEDBOAT ON A PAGE

[Home](../index.md) | [Docs](index.md) | [Guides](../guides/index.md) | [Ceremonies](../guides/ceremonies/index.md) | [Templates](../templates/index.md) | [Setup](../setup/index.md)

### Start less. Learn faster. Land more.

Speedboat helps AI-accelerated teams finish meaningful work, not just start more work. Each week, the team limits starts, makes Run visible, and proves what Landed.

Use this page as the cheat sheet. Use [Getting Started](../guides/getting-started.md) to start next week, and [Full Guide](model.md) when you want the full rationale, controls, and scaling patterns.

---

> **The core question:** What meaningful thing are we landing this week?

---

## The model

**Preview, Build, and Run are the work lanes. Land is the outcome layer.**

**PREVIEW**: Quick prototypes, PoCs, or demos to learn and enable conversations.
Max 3 active. 1–5 day timebox. Decision every Friday: kill, park, continue, or promote. Previews should not drift without a decision.
Two types: **Discovery** (should we build this?) and **Demo** (make it real for Sales/customers).

**BUILD**: Production-grade capability work. Max 3 active. Quality bar unchanged.
Sources: promoted Previews, committed roadmap, customer needs, platform necessities.
Big bets can span multiple weeks, but they should move through meaningful partial Landings rather than one invisible block of Build work.

A WIP item is not a subtask. It is a meaningful unit of work the team is steering: a prototype, a feature slice, a production change, or another outcome-sized piece of work.

**RUN**: Visible operational work. Split reactive (incidents, escalations) and proactive (debt, upgrades, automation). Aim ≤20%. Track honestly.

Those are the work lanes. Land sits above them as the outcome layer.

**LAND**: Prove progress. A Landing is a meaningful outcome: something reached a real beneficiary, or new evidence changed what happens next.

| Customer | Business | Platform | Decision |
|---|---|---|---|
| Feature live, beta, fix deployed | Demo ready, GTM enabled | Debt removed, risk reduced | Preview killed, parked, or promoted with learning |

Record weekly outcomes in the [Landing Log](../templates/landing-log.md).

## Team and roles

Speedboat works best with a small boat of about 4-5 engineers.

- **Product Lead** owns product priority and intended outcomes.
- **Captain** is the engineering lead for the boat, typically the tech lead, team lead, or engineering manager closest to the day-to-day work. They own boat health, WIP discipline, escalation, and making sure the Landing Log stays current.
- **Crew** is the rest of the engineering team. The Captain works with the crew, but carries explicit accountability for the health of the boat.

Product Lead is separate from the crew. Facilitation rotates, but accountability for the health of the boat does not.

---

## A normal week

Three weekly steering points keep the boat moving.

| | | |
|---|---|---|
| **Mon** | **Set Course** (30 min) | What are we landing this week? Confirm WIP. Set ownership. |
| **Wed** | **Course Check** (15 min) | Still on track? Unblock or adjust scope now. |
| **Fri** | **The Landing** (30 min) | What landed? Decide every Preview. Capture learning. |

Route Planning keeps the next few weeks shapeable.

| | | |
|---|---|---|
| **Every 2 weeks** | **Route Planning** (60 min) | Keep the next 2–4 weeks shaped enough that weekly steering does not become backlog grooming. |

Learning Review and Fleet Sync are periodic or adaptive loops.

| | | |
|---|---|---|
| **Every 4 weeks** | **Learning Review** (30 min) | What is the recent work teaching us about the model, WIP, Landing mix, and Run load? |

If you run multiple boats, add **Fleet Sync** every 2 weeks to handle dependencies, shared platform priorities, and cross-boat risks.

---

## Principles

1. Start less than you could
2. Make Run visible
3. Land outcomes, not activity

---

## Two rules

**Landing mix** — At least some Customer or Business Landings in any 4-week window. Platform-heavy by accident is a signal to course-correct.

**Exception protocol** — WIP limits can flex for urgent Run or escalations, but the team names what is paused to make room. Urgent Run doesn't violate Speedboat; hiding it does.

---

## Quick reference

If you're thinking:

- "I don't know if we should build this" -> Preview (Discovery)
- "Sales needs something to show" -> Preview (Demo)
- "We've committed to building this properly" -> Build
- "This broke / this is urgent" -> Run (Reactive)
- "We should fix this before it breaks" -> Run (Proactive)
- "This reached someone who benefits" -> Landing. Log it.

If you're not sure, it's probably a Preview.
