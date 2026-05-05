# Speedboat — Jira Board Configuration Guide

## Overview
This guide shows the easiest way to run Speedboat in Jira without admin access.

The default recommendation is:

- Use a **Kanban** board
- Scope the board to one team label
- Keep normal Jira columns such as **To Do / In Progress / Done**
- Use **labels** to distinguish Preview, Build, Run, and Landings

This is enough to start the model well. You do not need custom fields, custom workflows, or a dedicated Jira project for Week 1.

---

## Recommended setup

If you want Speedboat to be easy to adopt, use this setup:

- One board label for team membership, for example `speedboat-teamname`
- One work-type label on each issue: `preview`, `build`, or `run`
- Optional labels where helpful: `landing`, `discovery`, `demo`
- One shared Landing Log outside Jira

This gives you four benefits immediately:

- No Jira admin dependency
- No workflow redesign
- Easy team-level scoping
- Fast adoption this week

---

## Step 1: Create the board

When Jira asks whether to use **Scrum** or **Kanban**, choose **Kanban**.

Speedboat is continuous flow with a weekly steering rhythm. It is not sprint-based.

### What to choose on the board creation screen

For most teams, choose **Label**.

Use one label that means "this issue belongs on our Speedboat board", for example:

- `speedboat-personalize`
- `speedboat-analytics`

Then add that label to every issue that should appear on the board.

If your team already has a clean project boundary, **All work items from your space** can also work. But **Label** is the safest default when multiple teams share one Jira project.

### Naming the board

Use a simple name such as:

- `Speedboat - Personalize`
- `Speedboat - Analytics`

---

## Step 2: Keep the columns simple

Use normal Jira flow columns:

- **To Do**
- **In Progress**
- **Done**

You do not need special Speedboat columns to begin.

The columns answer: where is this work in execution?

The labels answer: what kind of work is this in the Speedboat model?

If your existing Jira workflow has extra statuses, map them into those three broad columns rather than redesigning the workflow up front.

---

## Step 3: Use labels for the Speedboat model

Add one of these labels to every issue on the board:

- `preview`
- `build`
- `run`

Optional labels:

- `landing` when something reached a meaningful outcome this week
- `discovery` for Discovery Previews
- `demo` for Demo Previews

### Recommended label rules

- Every issue should have exactly one of `preview`, `build`, or `run`
- Use `landing` only when the outcome has actually been reached
- Remove `landing` after the week ends if you only want it for temporary visibility, or keep it if you want historical filtering

Example:

- `speedboat-teamname`, `build`
- `speedboat-teamname`, `preview`, `discovery`
- `speedboat-teamname`, `run`

---

## Step 4: Configure swimlanes

If your Jira board supports **query swimlanes**, use them.

This is the easiest way to visualise Preview / Build / Run without changing workflows.

Create these swimlanes:

### Preview

```jql
labels = speedboat-teamname AND labels = preview
```

### Build

```jql
labels = speedboat-teamname AND labels = build
```

### Run

```jql
labels = speedboat-teamname AND labels = run
```

If your board filter already scopes to `speedboat-teamname`, you can shorten these to:

```jql
labels = preview
```

```jql
labels = build
```

```jql
labels = run
```

### What about Land?

Do **not** make Land a normal swimlane for everyday work.

Land is not where work sits. It is what you log when work reaches a meaningful outcome.

If useful, you can create a temporary quick filter for:

```jql
labels = landing
```

---

## Step 5: Add quick filters

Useful quick filters on the board:

| Label | JQL |
|---|---|
| Preview only | `labels = preview` |
| Build only | `labels = build` |
| Run only | `labels = run` |
| Landings this week | `labels = landing` |
| Discovery Previews | `labels = preview AND labels = discovery` |
| Demo Previews | `labels = preview AND labels = demo` |

If your board is not already scoped by the team label, add it into each query.

Example:

```jql
labels = speedboat-teamname AND labels = preview
```

---

## Step 6: First-week operating advice

If you need to start this week, the minimum is:

- Add the team label to all in-scope existing work
- Add one work-type label to each issue: `preview`, `build`, or `run`
- Pick 1-2 issues most likely to become Landings this week
- Start the ceremonies
- Log Landings in the [Landing Log](../templates/landing-log.md)

Do not wait for:

- custom fields
- workflow changes
- dashboards
- automation
- backlog cleanup

---

## Optional: fuller setup later

If the trial works and you want better reporting later, you can add:

- custom fields for category, preview type, landing type, and run type
- more precise JQL filters and dashboards
- explicit Preview / Build / Land statuses
- automation for Promoted / Landed transitions

But none of that is required to prove the model.

## Done!

If the board shows the right team's work, each issue has a Speedboat label, and the team can run Set Course / Course Check / The Landing, you are ready to start.