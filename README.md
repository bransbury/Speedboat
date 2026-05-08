# Speedboat

### Scrum was designed for a world where writing code was the expensive part. That world is gone.

In an AI-accelerated environment, teams do not automatically ship faster. They start more.

The cost of starting has collapsed. The cost of finishing has not. AI changed how we write software. Speedboat changes how we land it.

**Start less. Learn faster. Land more.**

Speedboat is a post-Scrum operating model for teams where AI has made starting cheap but finishing expensive.

It replaces sprint commitments with a weekly steering rhythm. It replaces velocity with meaningful outcomes. It replaces "how much can we start?" with a harder, better question:

> *What meaningful thing are we landing this week, and what do we need to learn or finish to make that happen?*

---

## How It Works

Speedboat has three work lanes and one outcome layer:

- **Preview:** quick prototypes, PoCs, or demos to learn fast
- **Build:** production-grade work that ships
- **Run:** operational work that keeps the lights on
- **Land:** the meaningful outcome when work reaches a real beneficiary

Work moves through three lanes, and the outcomes are logged as Landings:

| Element | What It Is | Constraints |
|---|---|---|
| **Preview** | Quick prototypes, PoCs, or demos to learn fast | Max 3 active. 1–5 day timebox. Decision every Friday. |
| **Build** | Production-grade work that ships | Max 3 active. Quality bar unchanged. Big bets can span multiple weeks, but should move through partial Landings. |
| **Run** | Operational work that keeps the lights on | Reactive + Proactive. Aim ≤20%. Track honestly. |
| **Land** | Meaningful outcomes reaching a real beneficiary | Customer, Business, Platform, or Decision. Logged weekly. |

Not all Landings mean the same thing. Customer Landings show delivered value. Business Landings show enablement. Platform Landings show capability and resilience. Decision Landings show learning. A healthy team may produce all four, but should not confuse learning or enablement with customer impact.

Three core ceremonies a week. Zero status updates.

Four lightweight ceremonies replace sprint planning and daily standups:

The default rhythm is Monday / Wednesday / Friday, but teams should shift the cadence to match their working week. The important pattern is start-of-week steering, mid-week course correction, and end-of-week Landing.

| | | |
|---|---|---|
| **Monday** | Set Course (30 min) | What are we landing this week? |
| **Wednesday** | Course Check (15 min) | Still on track? Adjust now. |
| **Friday** | The Landing (30 min) | What landed, who benefited, what did we learn? |
| **Fortnightly** | Route Planning (60 min) | Shape what's coming. What needs Preview before Build? |
| **4 wks** | **Learning Review** (30 min) | What is the recent work teaching us about WIP, Landing mix, Run load, and how the model is working? |

If you run multiple boats, add a lightweight **Fleet Sync** every two weeks: 30 minutes, one representative per boat plus product and engineering leadership, focused only on dependencies, shared platform priorities, and cross-boat risks.

New ideas should go into an **unshaped backlog** first. Route Planning shapes that backlog into Preview and Build candidates; urgent work uses Run or the exception protocol.

Speedboat is designed for small, nimble teams of 4–5 engineers. Fewer seats means less coordination overhead, faster decisions, and tighter ownership of what lands.

No standups. No points. No sprint commitments. No burndown charts. No velocity tracking. Just a relentless focus on landing meaningful work.

---

## What Speedboat Is Not

| | |
|---|---|
| **Not "move fast and break things"** | Preview can be rough. Build and Land meet production standards. |
| **Not one-week Scrum** | It's a steering rhythm for continuous flow, not a sprint under a different name. |
| **Not "ship every Friday or fail"** | A Landing can be a customer feature, a Sales demo, a platform improvement, or a decision to kill a bad idea. The ask is meaningful outcomes, not forced releases. |
| **Not anti-Scrum for the sake of it** | Scrum solved real problems. Speedboat is for teams where AI has changed the constraints Scrum was designed around. If Scrum is working for you, keep using it. |

---

## Who This Is For

- Engineering teams using AI tools (Copilot, Cursor, etc.) who notice they're producing more code but not shipping more value
- Teams where Scrum has degraded into sprint-shaped delivery without the discipline: no points, flexible scope, mixed work
- Leaders who want to run a low-risk trial of a different operating model without a transformation programme
- Anyone who's felt the gap between "we're building faster" and "customers are seeing more"

---

## Start Here

| You are… | Read this |
|---|---|
| A leader evaluating whether to try this | [Leadership Brief](docs/leadership-brief.md) |
| A team about to adopt Speedboat | [Getting Started](guides/getting-started.md) |
| An engineer wanting the 2-minute version | [One-Page Summary](docs/one-page-summary.md) |
| A team using AI agents heavily | [AI Agents in Speedboat](docs/ai-agents.md) |
| A facilitator running a ceremony | [Ceremony Guides](guides/ceremonies/) |
| Setting up your board | [Jira Setup](setup/jira.md) |
| Stuck or confused about something | [FAQ & Troubleshooting](docs/faq.md) |

---

## What's In This Repo

```
speedboat/
├── docs/
│   ├── model.md                    # The full operating model
│   ├── one-page-summary.md         # Printable one-pager
│   ├── ai-agents.md                # How AI agents fit within the lanes
│   ├── leadership-brief.md         # Proposal for leadership buy-in
│   └── faq.md                      # Common questions and troubleshooting
├── guides/
│   ├── getting-started.md          # Week 0 checklist: launch in a day
│   ├── which-lane.md               # Decision tree: where does this work belong?
│   ├── facilitation-rotation.md    # How to rotate ceremony facilitation
│   └── ceremonies/
│       ├── set-course.md           # Monday
│       ├── course-check.md         # Wednesday
│       ├── the-landing.md          # Friday
│       ├── learning-review.md      # Every 4 weeks
│       ├── route-planning.md       # Fortnightly, per boat
│       └── fleet-sync.md           # Fortnightly, multi-boat only
├── templates/
│   ├── landing-log.md              # Track what landed, for whom, and why
│   ├── weekly-snapshot.md          # Friday summary for your team channel
│   ├── monthly-stakeholder-summary.md # 4-week outward summary for leadership and stakeholders
│   ├── preview-decision-record.md  # Capture every Preview decision
│   ├── trial-evaluation.md         # End-of-trial readout structure
│   └── team-survey.md             # Anonymous team feedback survey
├── setup/
│   └── jira.md                     # Step-by-step board configuration
├── CHANGELOG.md
└── LICENSE                         # CC-BY-4.0
```

---

## Principles

1. Customer impact is the unit of progress
2. Start less than we think we can
3. Preview cheaply, decide quickly
4. Prioritise Landing over starting
5. Make trade-offs and Run work visible
6. Keep the quality bar unchanged
7. Use AI to accelerate work, not replace judgement
8. In short weeks, reduce scope, not discipline

---

## Roles

- **Product Lead:** owns product priority and intended outcomes.
- **Captain:** the engineering lead for the boat. Owns WIP discipline, escalation, incident trade-offs, and overall boat health.
- **Crew:** everyone contributes across Preview, Build, Run, and rotating facilitation.

Facilitation rotates, but the Captain remains accountable for board hygiene, ceremony quality, and keeping the boat healthy.

---

## Decision Rights

| Decision | Default owner |
|---|---|
| Intended Landing for the week | Product Lead and Captain together |
| Preview decision: kill / park / continue / promote | Product Lead and Captain together |
| Production readiness for Build | Captain / Engineering |
| Priority of what enters Preview or Build | Product Lead |
| Run prioritisation during incidents | Captain |

When Product Lead and Captain disagree, resolve it explicitly and quickly. If it remains unresolved by the end of the working day, escalate to the next product and engineering leaders rather than leaving work in limbo.

If you run multiple boats, use a lightweight Fleet Sync to handle cross-boat dependencies, shared platform priorities, and risks that affect more than one boat.

---

## Adapting Speedboat

This repo is a starting point, not a prescription. Things you should change for your context:

- **Team size:** Speedboat is designed for 4–5 engineers per team. If you have more, run multiple boats rather than one larger one.
- **WIP limits:** 3/3 assumes a team of 4–5. Adjust proportionally if your boat is smaller.
- **Ceremony timing:** Monday/Wednesday/Friday assumes a co-located or overlapping-timezone team. Shift as needed.
- **Landing types:** add types that matter to your business. Remove ones that don't.
- **Run target:** 20% is a starting point. If your system is unstable, it might be 40%. Be honest about it.
- **Trial length:** 4-6 weeks is enough to learn. Shorter is too noisy. Longer delays the decision.

Fork the repo. Make it yours. If you learn something useful, consider opening a PR or sharing what you changed.

---

## Licence

[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/) — use it, adapt it, share it. Attribution appreciated.