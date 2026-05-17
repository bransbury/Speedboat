# Speedboat — Which Lane?

[Home](../index.md) | [Docs](../docs/index.md) | [Guides](index.md) | [Ceremonies](ceremonies/index.md) | [Templates](../templates/index.md) | [Setup](../setup/index.md)

Use this when you're not sure where a piece of work belongs.

Preview, Build, and Run are the work lanes. Land is the outcome layer.

Land is not a lane you plan into. It is a meaningful outcome: something reached a real beneficiary, or new evidence changed what happens next.

This guide answers **what kind of work this is**. It does not decide whether the work should enter the system immediately. Non-urgent new work should go into the unshaped backlog until Route Planning shapes it.

It also does not change based on whether a human or an AI agent did the work. Agent-assisted work still belongs in Preview, Build, or Run based on intent and risk.

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
  ├─ Has something just reached a real beneficiary, or did new evidence change what happens next?
  │   └─ YES → Log a **Landing**
  │
  └─ Still not sure?
      └─ It's probably a **Preview**. Start small, learn, decide Friday.
```

---

## Quick Rules of Thumb

If you're thinking:

- "I don't know if we should build this" -> Preview (Discovery)
- "Sales needs something to show" -> Preview (Demo)
- "We've decided to build this properly" -> Build
- "This broke / this is urgent" -> Run (Reactive)
- "We should fix this before it breaks" -> Run (Proactive)
- "This reached a real beneficiary, or we learned something that changes what happens next" -> Landing

If you're not sure, it's probably a Preview.

---

## Common Mistakes

- Don't put exploratory work in Build.
  Do treat it as a Preview first when there are still open questions.
- Don't let Run work stay invisible.
  Do make it a first-class card, tag it, and track it.
- Don't skip the Landing log.
  Do log it when work reaches a real beneficiary, or when new evidence changes what happens next.
- Don't let a Preview run for 2+ weeks without a decision.
  Do raise it on Friday and decide whether it is Build in disguise or should be killed.
