# Speedboat — Weekly Snapshot Template

Post this to the team channel every Friday after The Landing ceremony. Takes ~5 minutes to fill in.

---

## Template

```
📍 Speedboat — Week [N] Snapshot
   [Date range: Mon DD – Fri DD Mon YYYY]

🟢 LANDED
   • [Title] — [Landing Type] — [one-line outcome]
   • [Title] — [Landing Type] — [one-line outcome]

🔵 PREVIEW DECISIONS
   • [Title] → Kill | Park | Continue | Promote — [one-line rationale]
   • [Title] → Kill | Park | Continue | Promote — [one-line rationale]

🔴 INTENDED BUT DIDN'T LAND
   • [Title] — [why: blocked on X / scope larger than expected / paused for urgent Run]

⚙️ RUN
   Reactive: [brief list or "none"]
   Proactive: [brief list or "none"]
   Estimated Run %: [X]%

📊 WIP
   Preview: [N] active (limit: 3)
   Build: [N] active (limit: 3)

💡 KEY LEARNING
   [One or two sentences. What did we learn this week that changes how we think about upcoming work?]
```

---

## Example (filled in)

```
📍 Speedboat — Week 3 Snapshot
   12 – 16 May 2026

🟢 LANDED
   • Bulk export API — Customer — Enterprise customers can now export >10k rows; unblocks 3 renewal conversations
   • Updated onboarding flow copy — Business — Sales demo now includes revised first-run experience

🔵 PREVIEW DECISIONS
   • AI summary feature → Kill — Latency too high for inline UX (~800ms). Parked until model improves.
   • Dashboard redesign → Promote — Validated with 3 customers in demo. Moving to Build with Partial Reuse label.

🔴 INTENDED BUT DIDN'T LAND
   • Webhook retry logic — blocked on decision from Platform team re: retry strategy. Carrying to W4.

⚙️ RUN
   Reactive: P1 login timeout (resolved Tues, ~4h)
   Proactive: Dependency upgrade for auth library
   Estimated Run %: ~15%

📊 WIP
   Preview: 2 active (limit: 3)
   Build: 3 active (limit: 3)

💡 KEY LEARNING
   AI summary PoC taught us that any inline AI feature needs <200ms round-trip to feel native.
   We should add latency budget as a Preview exit criterion for AI features going forward.
```

---

## Tips

- **Keep it short.** This is a signal, not a report. If it takes more than 5 minutes, you're over-thinking it.
- **Be honest about 🔴.** Missed landings aren't failures — hiding them is. Naming them early prevents surprises.
- **Run % is an estimate.** Don't spend time calculating it precisely. Rough is fine. The trend over weeks is what matters.
- **Post it publicly.** The snapshot is for the team, but also for anyone who wants to see what the team is doing without attending ceremonies.
- **Link to the Landing Log.** If someone wants detail, point them to the full log rather than expanding the snapshot.