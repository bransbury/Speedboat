# Leadership Brief: Speedboat

[Home](../index.md) | [Docs](index.md) | [Guides](../guides/index.md) | [Ceremonies](../guides/ceremonies/index.md) | [Templates](../templates/index.md) | [Setup](../setup/index.md)

**An operating model for AI-accelerated software teams**

| | |
|---|---|
| **Author** | Marcus Bransbury |
| **For** | VP Engineering / CPTO |
| **Status** | Proposal: low-risk 4–6 week trial |
| **Length** | 3-minute read |

---

## Executive summary

Speedboat helps AI-accelerated teams finish meaningful work, not just start more work.

It gives teams a simple weekly loop: limit starts, make Run visible, and prove what Landed.

AI has materially changed the economics of software delivery on our team. Reading code, prototyping, refactoring, and producing demoable software are all dramatically faster. Our current loose two-week Scrum was designed for a slower implementation phase and risks turning that AI-driven speed into more half-finished work, more prototypes, more demos, without proportionally more customer impact.

Speedboat is a lightweight weekly operating model with three work lanes (Preview, Build, Run) and one outcome layer (Land). It runs on a steering rhythm of Monday Set Course, Wednesday Course Check, Friday Landing, and fortnightly Route Planning.

I've aligned with our Product lead on the Preview and Landing model; they're supportive of running this as a trial.

I'd like to run a 4–6 week trial inside my engineering group and report back. The trial is low-risk, requires no tooling investment, and is reversible. The intent is to learn whether this approach delivers more meaningful outcomes per week than our current sprint model.

---

## Why now

Our existing process (sprint-shaped, two-week, mixed work, no points) is workable but built around an older constraint: that implementation was the expensive part. AI has weakened that constraint. The new bottlenecks are:

- Are we building the right thing?
- Are we finishing what matters?
- Are we learning fast enough?
- Are we keeping production safe and maintainable?

Without a deliberate operating model, AI acceleration tends to create the opposite of speed: more parallel starts, more prototypes that stall, more accidental productionisation of PoC code, and more operational drag. Speedboat is designed to harness AI acceleration without letting it overwhelm the system.

The cost of starting has collapsed. The cost of finishing (judgement, integration, review, rollout, support, learning) has not. That asymmetry is exactly what Speedboat is built to manage.

---

## The model in one page

### Work lanes and outcome layer

| Element | What It Is | Constraints |
|---|---|---|
| **Preview** | Quick prototypes, PoCs or demos to learn and enable conversations | Max 3 active. 1–5 day timebox. Decision every Friday. |
| **Build** | Production-grade work | Max 3 active. Standards unchanged. |
| **Run** | Visible operational work, split reactive/proactive | Aim 20% capacity, track honestly. |
| **Land** | A meaningful outcome: something reached a real beneficiary, or new evidence changed what happens next | Customer, Business, Platform, or Decision. Logged weekly. |

Not all Landings mean the same thing. Customer Landings show delivered value. Business Landings show enablement. Platform Landings show capability and resilience. Decision Landings show learning. A healthy team may produce all four, but learning or enablement should not be mistaken for customer impact.

### Weekly rhythm: replaces sprint planning and standups

The default rhythm is Monday / Wednesday / Friday, but teams should shift the cadence to match their working week. The important pattern is start-of-week steering, mid-week course correction, and end-of-week Landing.

| Ceremony | Duration | Purpose |
|---|---|---|
| Monday: Set Course | 30 min | Choose this week's intended Landing. |
| Wednesday: Course Check | 15 min | Adjust before the week is lost. |
| Friday: The Landing | 30 min | Show outcomes, decide every Preview, capture learning. |
| Fortnightly: Route Planning | 60 min | Shape upcoming work and what needs Preview. |

The core question shifts from "What tickets are we committing to this sprint?" to "What meaningful thing are we landing this week?"

---

## What leadership should see

If Speedboat works, the externally visible signals (the things you and the wider business will notice) are:

- A more consistent cadence of meaningful outcomes reaching customers, Sales, or the platform. Fewer weeks where the team is busy but nothing of substance lands.
- Faster time from roadmap idea to a credible demo Sales can put in front of a customer.
- Sharper conversations about trade-offs. Quality, debt, capacity, and Run load become visible instead of inferred.

Quality, security, and production standards do not change. Preview can be rough because it is for learning. Build and Land work continue to meet the same bar.

---

## Trial proposal

| Week | Focus |
|---|---|
| Week 0 | Introduce model to the team. Address concerns. Secure explicit opt-in. Agree trial period. |
| Week 1 | Start lightweight. Set up board. Run Set Course / Course Check / Landing. Limit WIP. Avoid over-documenting. |
| Week 2 | First Route Planning session. Shape upcoming work. Identify Preview candidates. |
| Weeks 3–4 | Tune and evaluate. Inspect WIP, Landings, ceremony timings. Gather team, Product, and Sales feedback. |
| Final week | Decide: continue, adjust, expand, or stop. Codify what we keep. |

---

## How we'll know it's working

Speedboat will not be measured on velocity. I'll track a small set of primary indicators that decide the trial, plus a wider set of diagnostic signals to understand why.

### Primary indicators: these decide whether the trial continues

- **Cadence and mix of Landings.** Meaningful Landings per week trend up, with at least some Customer or Business Landings in any rolling 4-week window.
- **Time from roadmap idea to a credible demo** measurably shortens.
- **Quality and sustainability hold.** Escaped defects, rollback rate, production support load, and team focus do not degrade.

If any primary indicator moves the wrong way by the evaluation week with no good explanation, we adjust or stop the trial.

### Diagnostic indicators: tracked internally to explain movement in the primary set

A WIP item is not a subtask. It is a meaningful unit of work the team is steering: a prototype, a feature slice, a production change, or another outcome-sized piece of work.

- WIP held within limits (≤3 Preview, ≤3 Build) for most of the trial.
- Every active Preview receives a Friday decision. No zombie Previews carry past one continuation.
- Started-vs-Landed ratio trends toward 1.0. We stop starting more than we finish.
- Run is visible and split reactive/proactive, instead of hiding inside Build.
- Preview kill rate is non-zero. The team is willing to stop work, not just start it.

Diagnostics are for the team and for me; only the primary indicators are reported up.

### Decision rights

| Decision | Default owner |
|---|---|
| Intended Landing for the week | Product and Engineering together |
| Preview decision: kill / park / continue / promote | Product and Engineering together |
| Production readiness for Build | Engineering |
| Priority of what enters Preview or Build | Product |
| Run prioritisation during incidents | Engineering |

---

## Two policy notes

### Landing mix

Over any 4-week window we expect at least some Customer or Business Landings, unless the team has explicitly chosen a Platform/Run-heavy period. Platform-heavy by accident is a signal to course-correct.

### Exception protocol

WIP limits are a steering rule, not a wall. Urgent Run, customer escalations, and leadership overrides are allowed, but the team names what is being paused to make room. The limit applies to meaningful work items, not individual subtasks. Urgent Run does not violate Speedboat; hiding it does.

---

## Risks and mitigations

| Risk | Mitigation |
|---|---|
| Sales over-promises based on a Demo Preview. | Demo Previews carry explicit caveats. Product and Engineering jointly approve what's shown and what can be promised. Roadmap commitment is a separate decision. |
| Quality drops under weekly cadence. | Build and Land standards are unchanged. Preview is the only lane where rough work is acceptable. Promotion to Build requires Engineering sign-off. |
| The team perceives this as "one-week sprints." | Speedboat is a steering rhythm, not a commitment cycle. Weekly framing is for direction-setting, not deadline pressure. Short weeks reduce scope, not discipline. |
| Prototype code accidentally ships to production. | Every promoted Preview carries an explicit code-reuse label: Throwaway / Reference / Partial Reuse / Foundation. Engineering owns the readiness gate. |
| Team feels constantly rushed. | WIP limits, fewer ceremonies, and explicit short-week handling are designed to reduce fragmentation, not increase pressure. |
| Tech debt gets ignored. | Run is a first-class lane and visible in the same operating model. Tech debt can Land as a Platform Landing when it reduces risk or unlocks delivery. |

---

## The ask

Endorsement to run a 4–6 week trial inside my engineering group, with the following commitments from me:

- No additional tooling spend or process overhead on other teams during the trial.
- Same quality, security, and release standards as today.
- Honest, evidence-based readout at the evaluation point with the metrics above.
- A clear go / adjust / stop recommendation at the end of the trial.

If the trial is successful, I'll propose how (or whether) to extend it to other teams. If it isn't, we revert with no residual cost.

---

## Appendix

The full [operating model](model.md), [ceremony guides](../guides/ceremonies/), and [templates](../templates/) are available in this repository. Happy to walk through any of it in more depth.
