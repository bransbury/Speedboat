# Preview Decision Record

Use this to capture the Friday decision for each Preview. One record per Preview, updated each Friday until the Preview reaches a terminal state (killed, parked, or promoted).

---

## Template

Copy this for each Preview:

```
## [Preview Title]

**Type:** Discovery / Demo
**Started:** [Date]
**Timebox:** [End date]
**Owner:** [Name]

### Summary
[One or two sentences: what were we trying to learn or demonstrate?]

### Week 1 Decision
**Decision:** Kill / Park / Continue / Promote
**Rationale:** [One sentence: why this decision?]
**If Continue:** New timebox end date: [Date]. This is the final continuation.

### Week 2 Decision (if continued)
**Decision:** Kill / Park / Promote
**Rationale:** [One sentence]

### Outcome
**Code-Reuse Label (if promoted):** Throwaway / Reference / Partial Reuse / Foundation
**Key learning:** [What did we learn that we didn't know before?]
**Next step:** [Build item created / parked for revisit in Route Planning / nothing]
```

---

## Filled Example

```
## AI-powered search suggestions

**Type:** Discovery
**Started:** 2026-05-05
**Timebox:** 2026-05-09
**Owner:** Sarah

### Summary
Exploring whether we can generate meaningful search suggestions using the existing embeddings index, and whether latency is acceptable for inline display.

### Week 1 Decision
**Decision:** Continue
**Rationale:** Promising results on relevance but latency is ~600ms. Need 2 more days to test with cached embeddings.
**If Continue:** New timebox end date: 2026-05-14. This is the final continuation.

### Week 2 Decision
**Decision:** Kill
**Rationale:** Cached approach brought latency to ~350ms, still above the 200ms threshold for inline UX. Not viable without a fundamentally different architecture. Parking the idea until model serving improves.

### Outcome
**Code-Reuse Label:** N/A (killed)
**Key learning:** Any inline AI feature needs <200ms round-trip to feel native. Our current embedding infrastructure can't serve this use case without a dedicated low-latency layer.
**Next step:** Nothing immediate. Revisit if we invest in a real-time serving tier.
```

---

## Where to store these

Pick one approach and stick with it:

| Option | Pros | Cons |
|---|---|---|
| Fields on the Jira card | Lives with the work item. Easy to filter and report. | Limited space for rationale and learning. |
| This template in a wiki/Confluence page | Room for detail. Easy to review historically. | Separate from the board. Might get forgotten. |
| A running log (like the Landing Log) | Single place to see all decisions. Good for evaluation. | Needs discipline to maintain. |

Whichever you choose, the non-negotiable is: **every active Preview gets a recorded decision every Friday.** The format is less important than the habit.

---

## Decision Guide

| Decision | Use when | What happens next |
|---|---|---|
| **Kill** | Idea disproven, not viable, not valuable enough to pursue | Log the learning. Card moves to Killed. Record a Decision Landing. |
| **Park** | Interesting but not now. Timing, capacity, or dependency issue. | Log why. Card moves to Parked. Revisit in Route Planning. |
| **Continue** | Needs ≤1 more week to reach a clear decision point | Set a new timebox. **This is the last continuation.** Next Friday it must be killed, parked, or promoted. |
| **Promote** | Validated and worth building properly | Assign a Code-Reuse Label. Create a Build card. Preview card moves to Promoted. |

### Code-Reuse Labels (for promoted Previews)

| Label | Meaning |
|---|---|
| **Throwaway** | The Preview code served its purpose. Build from scratch. |
| **Reference** | Use the Preview as a reference for patterns and approach, but don't copy code directly. |
| **Partial Reuse** | Some modules or logic can be carried forward. Engineering identifies which parts. |
| **Foundation** | The Preview is solid enough to build on directly. Needs hardening, tests, and production standards applied. |

The label prevents the most dangerous failure mode: prototype code quietly becoming production code without anyone explicitly deciding that's OK.