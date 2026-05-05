# Speedboat — Which Lane?

Use this when you're not sure where a piece of work belongs.

Preview, Build, and Run are the work lanes.

Land is not a lane you plan into. It's what you log when work reaches a meaningful outcome.

---

```
START
  │
  ├─ Is this an urgent incident, bug, escalation, or emergency?
  │   └─ YES → **Run (Reactive)**
  │
  ├─ Is this planned maintenance, tech debt, dependency upgrade, or infra improvement?
  │   └─ YES → **Run (Proactive)**
  │
  ├─ Are we exploring whether we should build this? (Feasibility, appetite, unknowns)
  │   └─ YES → **Preview (Discovery)**
  │
  ├─ Are we making something demoable for Sales, a customer conversation, or stakeholder buy-in?
  │   └─ YES → **Preview (Demo)**
  │
  ├─ Is this committed, production-grade work with clear scope?
  │   └─ YES → **Build**
  │
  ├─ Has something just reached its intended beneficiary?
  │   └─ YES → Log a **Landing**
  │
  └─ Still not sure?
      └─ It's probably a **Preview**. Start small, learn, decide Friday.
```

---

## Quick Rules of Thumb

| Signal | Lane |
|---|---|
| "I don't know if we should build this" | Preview (Discovery) |
| "Sales needs something to show" | Preview (Demo) |
| "We've decided to build this properly" | Build |
| "This broke / this is urgent" | Run (Reactive) |
| "We should fix this before it breaks" | Run (Proactive) |
| "This is live / this reached someone" | Landing |

---

## Common Mistakes

| Mistake | Correction |
|---|---|
| Putting exploratory work in Build | If there are open questions about whether to build it, it's a Preview first |
| Treating Run work as invisible | Run is a first-class lane — make it a card, tag it, track it |
| Skipping the Landing log | If it reached a beneficiary, log it. Landings are how we measure progress. |
| Preview that's been running 2+ weeks | It's either Build in disguise or it needs to be killed. Raise it Friday. |