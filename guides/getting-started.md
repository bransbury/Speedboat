# Getting Started with Speedboat

This is your Week 0 checklist. Everything you need to go from "we're trying this" to "we're running it" in a single day.

**Time to set up:** ~2 hours if you can edit your board yourself; longer if you need Jira admin help or workflow changes.
**Prerequisite:** You've read the [One-Page Summary](../docs/one-page-summary.md) and your leadership has endorsed a trial (see [Leadership Brief](../docs/leadership-brief.md) if you need to make the case).

---

## Before You Start

Make sure you can answer these questions:

| Question | Why it matters |
|---|---|
| How long is the trial? | We recommend 4 weeks. Four iterations is enough to know whether the rhythm is working, without dragging out a decision. |
| Does the team know this is coming? | Speedboat requires opt-in, not mandate. Introduce the idea before configuring the board. |
| Is Product aligned? | Speedboat depends on Product and Engineering collaborating on Previews and Landing decisions. A one-line alignment is enough. A formal sign-off is not required. |
| What's your current WIP? | Before you set limits, know your starting point. Count active items right now. If it's 12, getting to 6 will feel like a real change. |

---

## Week 0 Checklist

### Minimum viable rollout

If you want the smallest possible version for Week 1, start with this:

- [ ] One board with Preview, Build, Run, and a visible way to mark Landings
- [ ] One [Landing Log](../templates/landing-log.md)
- [ ] One [Weekly Snapshot](../templates/weekly-snapshot.md)
- [ ] One shared understanding of WIP limits and Preview decisions

Do not wait for perfect dashboards, automation, or backlog cleanup. Week 1 should optimise for visibility, not tooling polish.

### Understand the model

- [ ] Read the [One-Page Summary](../docs/one-page-summary.md) (~2 min)
- [ ] Read the [full model](../docs/model.md) if you want the reasoning behind the design (~10 min)
- [ ] Review the [Which Lane?](which-lane.md) decision tree. Make sure the lane boundaries feel clear to you before explaining them to the team.
- [ ] Decide your boat boundaries if your wider group is larger than 5 engineers.

### Set up the board

- [ ] Follow the [Jira Setup Guide](../setup/jira.md) (or adapt for your tool)
- [ ] Configure columns and WIP limits first; add custom fields, filters, and dashboards if you have the access and time
- [ ] If Jira admin changes are slow, start with an existing board plus labels or conventions and tighten the setup later
- [ ] Move existing in-flight work into the appropriate lanes. Don't wait for a clean start.

### Set up tracking

- [ ] Create your [Landing Log](../templates/landing-log.md) (spreadsheet, Confluence, Notion, wherever your team lives)
- [ ] Bookmark the [Weekly Snapshot](../templates/weekly-snapshot.md) template
- [ ] Decide where snapshots will be posted (Slack channel, Teams, email, pick one)

### Set up the rhythm

- [ ] Add ceremonies to the team calendar:

| Ceremony | When | Duration | Invite |
|---|---|---|---|
| Set Course | Monday morning | 30 min | Whole team |
| Course Check | Wednesday midday | 15 min | Whole team |
| The Landing | Friday afternoon | 30 min | Whole team + optional stakeholders |
| Route Planning | Every other week | 60 min | Engineering + Product |

- [ ] Fill in the [Facilitation Rotation](facilitation-rotation.md) schedule for the trial period
- [ ] Print or bookmark the ceremony guides ([Monday](ceremonies/set-course.md) · [Wednesday](ceremonies/course-check.md) · [Friday](ceremonies/the-landing.md) · [Fortnightly](ceremonies/route-planning.md))

### Introduce to the team

- [ ] Walk through the one-page summary together
- [ ] Explain the three work lanes and the Land outcome layer. Use the [Which Lane?](which-lane.md) decision tree for concrete examples from your own backlog.
- [ ] Be clear about what's changing (ceremonies, WIP limits, Landing focus) and what's not (quality bar, release standards, who decides what to build)
- [ ] Address concerns openly. The common ones:
  - *"This feels like one-week sprints."* It's a steering rhythm, not a commitment cycle.
  - *"What if we can't land something every week?"* A Decision Landing (killing a bad Preview) counts. The ask is meaningful, not forced.
  - *"What about my ongoing work?"* Move it into the right lane. Nothing resets to zero.
- [ ] Agree on the trial length (4 weeks recommended)
- [ ] Secure explicit opt-in. The team should want to try this, not feel it's being imposed.

### Pick the first week's intended Landings

Before the first Set Course, look at your current in-flight work and choose 1-2 intended Landings for Week 1.

- [ ] Pick the items most likely to reach a real beneficiary this week
- [ ] Prefer something already in motion over something new and hypothetical
- [ ] If nothing can realistically land, choose the smallest meaningful partial outcome or an explicit Decision Landing
- [ ] Name what you will not start yet

---

## Week 1: Go

You are not trying to be perfect. You are trying to start the rhythm.

- [ ] **Monday:** Run Set Course. Pick 1–2 intended Landings for the week. Don't overthink it.
- [ ] **Monday:** Check WIP. If you're above the limits, don't panic. Name what you intend to finish before starting anything new.
- [ ] **Wednesday:** Run Course Check. Keep it to 15 minutes. Ask: "Red, amber, or green on each intended Landing?"
- [ ] **Friday:** Run The Landing. Walk what landed. Decide every active Preview. Post your first Weekly Snapshot.
- [ ] **Friday:** Update the Landing Log.
- [ ] **After Friday:** Resist the urge to retrospect on the process itself. You have one data point. The process will feel clunky. That's fine. Give it time.

### What "good" looks like in Week 1

- The team can name what lane their work is in
- WIP limits are visible, even if not yet respected perfectly
- At least one thing landed (any type)
- Every active Preview got a Friday decision
- The board reflects reality

### What "good" does NOT look like in Week 1

- Every ceremony ran perfectly to script
- WIP was within limits all week
- Multiple Customer Landings
- The team loves the new process

Give it time. Week 1 is about starting the habit, not proving the model.

---

## Week 2 and Beyond

- [ ] **Week 2:** Run your first Route Planning session. Shape the next 2–4 weeks. Identify what needs a Preview before committing to Build.
- [ ] **Weeks 2–3:** Tune. Adjust ceremony timing if needed. Fix confusion about which lane work belongs in. Watch for zombie Previews.
- [ ] **Week 3:** Prepare for evaluation. Bookmark the [Trial Evaluation Template](../templates/trial-evaluation.md). Start gathering data from the Landing Log, snapshots, and board.
- [ ] **Week 4:** Evaluate. Fill in the trial evaluation. Run the [Team Survey](../templates/team-survey.md). Gather Product and Sales feedback. Decide: continue, adjust, expand, or stop.

---

## Common Week 1 Problems

| Problem | What to do |
|---|---|
| WIP is way over the limit | Don't force-stop work. Name the excess, finish what you can, and respect the limits for new starts. It normalises within 1–2 weeks. |
| Nobody landed anything | That's fine for Week 1. Check: did you set an intended Landing on Monday? Was it realistic? Adjust ambition, not the model. |
| "I don't know which lane this is" | Use the [Which Lane?](which-lane.md) decision tree. If it's genuinely ambiguous, default to Preview. |
| A P1 incident blew up the week | That's Run (Reactive). Name what got paused. This is Speedboat working as intended: making trade-offs visible, not pretending they don't happen. |
| The team thinks this is just one-week sprints | Reinforce: there is no sprint commitment. Monday sets direction. Friday shows outcomes. Nothing is "failed" if it didn't land. It carries forward with a reason. |
| Someone asks "where are the story points?" | Gone. Speedboat measures Landings (outcomes), not effort estimates. If this feels uncomfortable, that discomfort is worth discussing openly. |

---

## You're Ready

The most important thing in Week 1 is not running the model perfectly. It's starting the rhythm and making work visible. Everything else can be tuned.

If you get stuck, check the [FAQ](../docs/faq.md). If something's missing from this repo, [open an issue](../../issues).

Good luck. Start less. Learn faster. Land more.