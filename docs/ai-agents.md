# AI Agents in Speedboat

Use this guide if your team is using autonomous or semi-autonomous AI agents alongside Speedboat.

The short version: AI agents can accelerate work inside every lane, but they do not change who owns decisions or lower the finishing cost.

---

## Core principle

AI agents are accelerators, not owners.

They can explore, draft, compare, generate, refactor, summarise, and automate parts of the work. They do not own product judgement, production readiness, integration risk, rollout decisions, or accountability for what lands.

Speedboat already assumes that starting work is cheap and finishing work is expensive. AI agents make that asymmetry stronger.

If agents generate more code, prototypes, fixes, docs, or upgrade proposals than the team can properly review and land, the system slows down. The queue moves from "work to start" to "work that now needs judgement, integration, and review."

The quality bar stays the same.

---

## Preview

Preview is where agent autonomy is most naturally useful.

AI agents can:

- generate quick prototypes or PoCs
- explore multiple approaches in parallel
- compare implementation options
- produce demo-ready artifacts for discussion
- summarise findings and trade-offs

Human ownership stays on the decision:

- Should we build this?
- What did we learn?
- Do we kill, park, continue, or promote?

Treat agent-generated Preview output as disposable by default. Do not promote it into Build just because it appeared quickly. Promote it only when the team deliberately decides it is worth building properly.

---

## Build

AI agents are most useful in Build when the task is bounded and the acceptance criteria are clear.

Good candidates include:

- test generation and test expansion
- migration scripts
- repetitive refactors
- boilerplate and scaffolding
- documentation drafts
- code search and comparison work

Human ownership stays on:

- architecture and trade-offs
- integration with the rest of the system
- production readiness
- review quality
- rollout and support impact

The main failure mode is overproduction. If agents create more candidate changes than the team can review and integrate well, Build WIP rises in disguise. Treat review and integration as real work, not as free follow-up.

---

## Run

AI agents can make Run work faster and more proactive.

Useful patterns include:

- triaging alerts
- summarising incidents
- identifying likely root causes
- drafting remediation options
- proposing dependency upgrades
- generating low-risk maintenance changes for review

Human ownership stays on:

- deciding what action to take
- deciding what gets deployed
- deciding whether a fix is safe enough to roll out
- deciding what follow-up work is needed

Do not let automation blur the deployment decision. Faster triage is good. Unowned rollout risk is not.

---

## Guardrails

- Keep agent-generated work inside the same WIP limits as any other work.
- Prefer agents for bounded tasks with clear success criteria.
- Count review, integration, and validation as real effort.
- Do not treat agent output as production-ready by default.
- Do not let Preview artifacts quietly become Build code.
- Do not let Run automation bypass human deployment judgement.

---

## Good questions to ask

- "Is this reducing time to learning, or just generating more output?"
- "Is this task bounded enough for an agent to help safely?"
- "What review and integration work are we creating downstream?"
- "Would we still trust this change if a human had to explain and support it tomorrow?"
- "Are we speeding up finishing, or just speeding up starting?"

---

## In one sentence

AI agents fit well inside Speedboat when they help the team learn faster, implement bounded work faster, and triage Run faster without weakening human ownership of quality, integration, and rollout.