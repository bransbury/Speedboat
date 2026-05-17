# Speedboat — Landing Log

[Home](../index.md) | [Docs](../docs/index.md) | [Guides](../guides/index.md) | [Ceremonies](../guides/ceremonies/index.md) | [Templates](index.md) | [Setup](../setup/index.md)

This is the single weekly output for Speedboat.

Use it as a weekly template. Create one copy per week, or duplicate the Week section inside one running doc or spreadsheet.

The facilitator may update it live, but the Captain is accountable for making sure the log stays current.

Start with the simple weekly log below. Add the optional detail only when the team needs it.

A Landing is a meaningful outcome: something reached a real beneficiary, or new evidence changed what happens next.

Use the last 4 Landing Logs when preparing the monthly stakeholder summary.

Replace the sample rows below with your own entries each week.

---

## Week [N] — [Date range]

### Landings

| Title | Landing Type | Beneficiary | Outcome |
|---|---|---|---|
| New feature live | Customer | All customers | New feature now generally available. |
| New feature flagged capability in production | Customer | Chosen partner accounts | New capability now in early access for chosen partner accounts. |
| Demo feature in production | Business | Sales engineers / pre-sales | Sales engineers can now demo the capability to prospects and existing customers. |
| Retry logic added to webhooks | Platform | Customers using webhooks (~30%) | Failures now auto-retry to avoid manual intervention and re-runs. |

---

## Add Later If Needed

If the team wants more detail after the first few cycles, add these sections.

### Optional: Preview Decisions

Record every Friday Preview decision here, or as fields on the Jira card. Pick one method and use it consistently.

| Date | Preview Title | Preview Type | Decision | Rationale | Code-Reuse Label | Learning |
|---|---|---|---|---|---|---|
| 2026-05-11 | AI Summary Feature | Demo | Promote | Demo feedback was very positive. | Foundation | Users responded strongly to seeing long updates summarized quickly, so the first Build slice should focus on summary quality and making the output easy to share. |
| | | Discovery / Demo | Kill / Park / Continue / Promote | | Throwaway / Reference / Partial Reuse / Foundation | |
| | | | | | | |
| | | | | | | |
| | | | | | | |

---

### Optional: Notes

- Estimated Run %:
- Key learning:

---

## How to Fill This In

- **Title:** Short name for the work (e.g., "Bulk export API", "Kill: AI summary feature")
- **Landing Type:** Customer (live to users), Business (Sales-ready, GTM-enabled), Platform (debt, observability, risk), Decision (Preview killed/parked/promoted)
- **Beneficiary:** Be specific — "Enterprise customers on Pro plan", "Sales team for Q3 pipeline", "Platform team (reduced incident risk)"
- **Outcome:** What's true now that wasn't before? One sentence.
- **Source:** If you add the optional field, note where the work originated.
- **Notes:** If you add the optional field, use it for rollout detail or useful follow-up context.
- **Learning (Preview log):** Even for promoted Previews, capture what you learned. Especially for killed ones.
