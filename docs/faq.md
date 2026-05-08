# FAQ and Troubleshooting

Common questions, misconceptions, and real problems that come up during adoption.

---

## Understanding the model

### "How is this different from one-week sprints?"

Sprints have a commitment at the start and a review at the end. If you don't deliver, the sprint "failed." Speedboat has no sprint commitment. The start-of-week ceremony sets a direction. The end-of-week Landing shows what happened. If something didn't land, it carries forward with a reason. There's no failure, just visibility.

The cultural difference: sprints optimise for predictability. Speedboat optimises for learning and finishing.

### "Why one week, not two?"

Because AI increases the rate of starting.

When starting gets cheaper, drift, mistaken commitment, and hidden WIP accumulate faster too. That means the steering loop has to get shorter.

One week is short enough to correct direction before waste compounds, but long enough to produce something meaningful. Two weeks is often too long in an environment where code, demos, and branches can proliferate in days.

The point of the weekly cadence is not pressure. It is faster steering.

### "What happened to story points?"

Gone. Speedboat measures outcomes (Landings), not effort estimates. If you want to understand throughput, look at the Started vs. Landed ratio and Build age over time. These tell you more than points ever did.

### "What if my team is bigger than 5?"

Split into multiple boats, each with its own board and rhythm. Keep Route Planning per boat, and add a lightweight Fleet Sync every two weeks for cross-boat dependencies, shared platform priorities, and multi-boat risks rather than scaling a single ceremony set.

### "How do multiple boats coordinate dependencies?"

Use Fleet Sync. Each boat sends one representative, usually the Captain, plus product and engineering leadership. The point is not status reporting. The point is to name cross-boat dependencies early, assign owners, and make shared risks visible before a boat is blocked.

Keep the ownership simple:

- The boat needing the dependency owns making the need explicit.
- The boat providing the dependency owns giving a realistic commit or decline.
- Leadership steps in only when priorities or risks cross boat boundaries.

If a dependency only affects one boat's internal planning, keep it in Route Planning. If it affects multiple boats, take it to Fleet Sync.

### "Do I need to change team structure to try this?"

Not necessarily; you can pilot the rhythm inside an existing group, but the model works best when a boat has clear ownership and limited coordination overhead.

### "Do we still have a backlog?"

Yes, but it's shaped differently. New ideas go into an **unshaped backlog** first. Route Planning (fortnightly) promotes non-urgent items from that backlog into a shaped queue of Preview and Build candidates for the next 2–4 weeks. Anything further out lives in your roadmap or product backlog as before. Speedboat doesn't replace product planning; it replaces sprint-level execution planning.

### "What happens when a new request arrives mid-week?"

First ask whether it is urgent.

- **Urgent:** treat it as Run or use the exception protocol. Name what gets paused.
- **Not urgent:** add it to the unshaped backlog and review it in the next Route Planning.

The Product Lead and Captain can triage new work between Route Planning sessions, but they should not quietly inject non-urgent work into Build mid-week.

### "Where do bugs go?"

Depends on severity and urgency:
- **Urgent/breaking:** Run (Reactive). Fix it now, name what gets paused.
- **Important but not urgent:** Run (Proactive). Schedule it visibly.
- **Found during Build:** Part of the Build item. Fix before Landing.
- **Customer-reported, non-urgent:** Triage in Route Planning. Might become a Build item or fold into existing work.

### "What about work that takes longer than a week?"

Build items often span multiple weeks. That's fine. The question isn't "did you finish in one week?" It's "are you making progress toward a Landing, and is there something meaningful we can land along the way?" Slice vertically where possible. If a Build item has been in progress for 3+ weeks with no partial Landing, it's probably too big.

### "What about a big bet that takes 2 months?"

Treat it as a multi-week initiative, not as one giant invisible Build item.

Keep the big bet visible as the umbrella outcome, but move the work through a series of partial Landings across the next Route Planning cycles.

Examples:

- an API live behind a feature flag
- an internal beta ready for use
- a migration path completed
- observability and rollback protections in place

Those count if they are meaningful to someone or if they materially reduce risk and unlock the next slice.

The rule is not "finish the big bet every week." The rule is "make the big bet visible and steerable through meaningful Landings along the way."

If a big bet has gone more than 2 weeks without any meaningful partial Landing, raise it in Route Planning and re-slice it.

### "Does this work for platform/infrastructure teams?"

The lanes and rhythm work for any team. The Landing types might shift: platform teams will have more Platform Landings and fewer Customer Landings, and that's expected. The key question remains the same: is meaningful work reaching its intended beneficiary?

---

## Common problems

### A Preview has been running for 2+ weeks

This is a Preview that should have been killed, promoted, or re-scoped. By design, Previews are 1–5 days with a maximum of one continuation. If it's been two weeks, one of these is true:

- It's actually Build work disguised as a Preview. Promote it (with the appropriate code-reuse label) or kill the Preview and create a proper Build item.
- The scope was too ambitious for a Preview. Kill it and start a smaller one that targets a specific decision.
- Nobody made a Friday decision. This is a process failure. The facilitator's job is to ensure every Preview gets a decision. No exceptions.

### We had 4 Decision Landings and no Customer Landings for three weeks

Decision Landings are real and valuable (they save the team from building the wrong thing). But if they're the only type landing for multiple weeks, something is off:

- Are Previews being promoted to Build? If not, the team might be in a loop of exploring without committing.
- Is Build work stalling? Check Build age and WIP. Something might be blocked or too large.
- Is the team avoiding production-grade work? Sometimes Preview feels safer because the quality bar is lower.

Raise this in Route Planning. Explicitly plan for at least one Customer or Business Landing in the next 2-week window.

### The team says this feels like one-week sprints

Usually means one of:
- Monday feels like sprint planning (too detailed, too many items)
- Friday feels like a judgement or performance review
- People feel "failed" when something doesn't land

Fix by reinforcing: Monday sets direction (not a commitment). Friday shows outcomes (not a scorecard). Nothing is failed; it carries forward with a reason. Also check whether you're overloading Monday with too many intended Landings. One or two is plenty.

### An urgent incident blew up our WIP limits

This is Speedboat working correctly. Run (Reactive) absorbs the incident. The team names what got paused. At the next Course Check or Set Course, acknowledge the impact and adjust the week's intended Landings. Don't pretend the incident didn't happen. Don't quietly drop planned work without saying so.

### Product wants to skip Preview and go straight to Build

Sometimes appropriate: if the work is well-understood, already validated by customer feedback, or a committed roadmap item with clear scope. The question to ask: "Do we have open questions about whether this is the right thing, or how to approach it?" If yes, it needs a Preview. If genuinely no, go straight to Build.

The risk of skipping Preview is building the wrong thing expensively. The risk of insisting on Preview for everything is slowing down obvious work. Use judgement.

### Someone finished their Build item mid-week and wants to start something new

Check the WIP limits first. If there's room (fewer than 3 Build items active), they can pull the next shaped item from Route Planning. If WIP is at the limit, they should help land something else that's in progress, do proactive Run work, or start a Preview. The principle: finishing is more valuable than starting.

### "We don't have enough work shaped for Monday"

This means Route Planning isn't generating enough ready candidates. Either:
- Bring more items to the next Route Planning session
- The team lead does a quick 15-minute shaping conversation mid-week
- Accept that some weeks are lighter and use the space for Proactive Run

Don't fill the gap by pulling in unshaped work. Add it to the unshaped backlog and shape it properly. Unshaped work expands, misses, and demoralises.

---

## Philosophical questions

### "Isn't this just Kanban with extra steps?"

Kanban provides flow mechanics (WIP limits, pull-based work). Speedboat adds: a specific lane structure designed for AI-era dynamics, a weekly steering rhythm, a Landing-based definition of progress, and an explicit Preview lane for cheap learning before expensive building. Think of it as Kanban's principles applied to a specific problem with opinionated defaults.

### "What if Scrum is working fine for my team?"

Keep using it. Speedboat is for teams where Scrum has degraded or where AI has changed the underlying constraints (starting is cheap, finishing is hard). If your team has healthy sprints, consistent delivery, and satisfied customers, you don't need this.

### "Can we use parts of Speedboat without adopting the whole thing?"

Yes. The most portable pieces:
- The three work lanes plus Land outcome framing (even within a sprint model)
- Friday Preview decisions (add to any existing cadence)
- The Landing Log (works alongside any process)
- The "start less, land more" principle (just a mindset shift)

But the pieces work best together. The rhythm reinforces the lanes, the lanes reinforce the principles.