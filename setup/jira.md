# Speedboat — Jira Board Configuration Guide

## Overview
This guide walks a Jira admin through setting up a Speedboat board from scratch. Time estimate: 20–30 minutes.

---

## Step 1: Create the Project (or reconfigure existing)

Use a **Kanban** project template (not Scrum). Speedboat is continuous flow, not sprint-based.

---

## Step 2: Custom Fields

Create the following custom fields (Text/Select as noted):

| Field Name | Type | Options | Used On |
|---|---|---|---|
| Lane | Single Select | Preview, Build, Land, Run | All issues |
| Preview Type | Single Select | Discovery, Demo | Preview items |
| Timebox End Date | Date | — | Preview items |
| Decision | Single Select | Kill, Park, Continue, Promote | Preview items |
| Decision Rationale | Short Text | — | Preview items |
| Code-Reuse Label | Single Select | Throwaway, Reference, Partial Reuse, Foundation | Promoted Previews |
| Landing Type | Single Select | Customer, Business, Platform, Decision | Land items |
| Beneficiary | Short Text | — | Land items |
| Outcome Statement | Short Text | — | Land items |
| Run Type | Single Select | Reactive, Proactive | Run items |
| Source | Single Select | Promoted Preview, Roadmap, Customer Need, Platform Necessity | Build items |

---

## Step 3: Board Columns

Configure the board with these columns (left to right):

| Column | Statuses Mapped | WIP Limit |
|---|---|---|
| **Preview — Active** | Preview Active | 3 |
| **Preview — Decision Pending** | Preview Decision Pending | — |
| **Build — Ready** | Build Ready | — |
| **Build — In Progress** | Build In Progress | 3 |
| **Build — Landing** | Build Landing | — |
| **Land — Pending** | Land Pending | — |
| **Land — Landed** | Land Landed | — |
| **Run** | Run Active | — |
| **Done** | Done, Killed, Parked | — |

### Swim Lanes
Configure swim lanes by the **Lane** field (Preview, Build, Land, Run) so the board visually groups work by type.

---

## Step 4: Statuses & Transitions

Create these statuses if they don't already exist:

**Preview:** Preview Active → Preview Decision Pending → Promoted / Parked / Killed
**Build:** Build Ready → Build In Progress → Build Landing → Done
**Land:** Land Pending → Land Landed
**Run:** Run Active → Done

Transition rules:
- Preview Active → Preview Decision Pending: triggered by Friday Landing ceremony
- Preview Decision Pending → Promoted: requires Code-Reuse Label to be set
- Build In Progress → Build Landing: requires tests passing / PR merged (optional automation)

---

## Step 5: Saved Filters (JQL)

Save these filters for ongoing use:

**Zombie Previews** (active > 5 working days with no decision):
```
Lane = Preview AND status = "Preview Active" AND created <= -5d
```

**Active WIP count:**
```
Lane in (Preview, Build) AND status in ("Preview Active", "Build In Progress")
```

**Landings this week:**
```
Lane = Land AND status = "Land Landed" AND resolved >= startOfWeek()
```

**Started vs Landed (last 4 weeks):**
```
-- Started:
created >= -4w AND Lane in (Preview, Build)
-- Landed:
Lane = Land AND status = "Land Landed" AND resolved >= -4w
```

**Run split:**
```
Lane = Run AND resolved >= startOfWeek() AND "Run Type" = Reactive
Lane = Run AND resolved >= startOfWeek() AND "Run Type" = Proactive
```

---

## Step 6: Dashboard

Create a dashboard called **"Speedboat — [Team Name]"** with these gadgets:

| Gadget | Source |
|---|---|
| Filter Results: Active WIP | Active WIP count filter |
| Two-Dimensional Filter: Landings by type by week | Landings filter, rows = week, columns = Landing Type |
| Filter Results: Zombie Previews | Zombie Previews filter |
| Pie Chart: Run Reactive vs Proactive | Run split filters |
| Created vs Resolved (last 6 weeks) | All project issues — shows Started vs Landed trend |

---

## Step 7: Quick Filters (Board Header)

Add these as quick filters on the board:

| Label | JQL |
|---|---|
| Preview only | `Lane = Preview` |
| Build only | `Lane = Build` |
| Run only | `Lane = Run` |
| This week's Landings | `Lane = Land AND resolved >= startOfWeek()` |
| Zombie Previews | `Lane = Preview AND status = "Preview Active" AND created <= -5d` |

---

## Done!
Pin the Board README (next artifact) in the project description or sidebar so the team has context.