# Speedboat

### Scrum was designed for a world where writing code was the expensive part. That world is gone.

AI has collapsed the cost of starting work. Reading code, prototyping, refactoring, generating tests, producing demo-ready software: what used to take a week now takes a day. What used to take a day takes an hour.

But finishing work is just as expensive as it ever was. Judgement, integration, review, rollout, support, learning. None of that got cheaper.

The result? Teams using Scrum in an AI-accelerated environment don't ship faster. They start more. More branches, more prototypes, more half-finished work, more demos that never become products, more sprints where the team is busy but nothing of substance reaches a customer.

**Speedboat is a post-Scrum operating model for teams where AI has made starting cheap but finishing expensive.**

It replaces sprint commitments with a weekly steering rhythm. It replaces velocity with meaningful outcomes. It replaces "how much can we start?" with a harder, better question:

> *What meaningful thing are we landing this week, and what do we need to learn or finish to make that happen?*

**Start less. Learn faster. Land more.**

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
| **Build** | Production-grade work that ships | Max 3 active. Quality bar unchanged. |
| **Run** | Operational work that keeps the lights on | Reactive + Proactive. Aim ≤20%. Track honestly. |
| **Land** | Meaningful outcomes reaching a real beneficiary | Customer, Business, Platform, or Decision. Logged weekly. |

Not all Landings mean the same thing. Customer Landings show delivered value. Business Landings show enablement. Platform Landings show capability and resilience. Decision Landings show learning. A healthy team may produce all four, but should not confuse learning or enablement with customer impact.

Four lightweight ceremonies replace sprint planning and daily standups:

The default rhythm is Monday / Wednesday / Friday, but teams should shift the cadence to match their working week. The important pattern is start-of-week steering, mid-week course correction, and end-of-week Landing.

| | | |
|---|---|---|
| **Monday** | Set Course (30 min) | What are we landing this week? |
| **Wednesday** | Course Check (15 min) | Still on track? Adjust now. |
| **Friday** | The Landing (30 min) | What landed, who benefited, what did we learn? |
| **Fortnightly** | Route Planning (60 min) | Shape what's coming. What needs Preview before Build? |

Speedboat is designed for small, nimble teams of 4–5 engineers. Fewer seats means less coordination overhead, faster decisions, and tighter ownership of what lands.

No points. No burndown charts. No sprint commitments. No velocity tracking. Just a relentless focus on landing meaningful work.

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
│       └── route-planning.md       # Fortnightly
├── templates/
│   ├── landing-log.md              # Track what landed, for whom, and why
│   ├── weekly-snapshot.md          # Friday summary for your team channel
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
2. Start less work than we think we can
3. Preview cheaply, decide quickly
4. Build fewer things at once
5. Prioritise Landing over starting
6. Make Run work visible
7. Use AI aggressively, but keep human ownership
8. Product owns value; Engineering owns production readiness
9. In short weeks, reduce scope, not discipline

---

## Decision Rights

| Decision | Default owner |
|---|---|
| Intended Landing for the week | Product and Engineering together |
| Preview decision: kill / park / continue / promote | Product and Engineering together |
| Production readiness for Build | Engineering |
| Priority of what enters Preview or Build | Product |
| Run prioritisation during incidents | Engineering |

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