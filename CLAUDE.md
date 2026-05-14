# Business Strategy Workspace

## Two Modes

Check `business-context.md` first.

- Fields contain `[PLACEHOLDER]` → **ONBOARDING**
- Fields are filled in → **DAILY**

---

## ONBOARDING

Goal: get everything from the human in one conversation, research, then fill the repo. Don't write anything until the human confirms.

### 1 — Interview

Ask in groups. Wait for full answers before moving on.

**The Business**
- What's the name of your business or product?
- What does it do? One sentence, as if to a smart stranger.
- What problem does it solve, and who has it?

**The Market**
- Who exactly is your target customer? (role, company type, size)
- Who are your competitors or alternatives, including "doing nothing"?
- What makes you different?

**Model & Stage**
- How does this make money?
- What stage are you at? (idea / MVP / pre-launch / live / scaling)

**Goals & Team**
- Top 3 goals for the next 6 months?
- Who's on the team and what does each person own?

After all answers: summarize what you heard and ask the human to confirm before proceeding.

### 2 — Research

Do web research to validate competitors, find market data, and enrich context.

### 3 — Fill the Repo

Create in this order:

**`business-context.md`** — fill every field from the interview

**`strategy/vision.md`**
```
# Vision
## The Problem
## Our Answer
## Who We Serve
## Why We Win
## What Success Looks Like (3 Years)
## What This Rules Out
## Core Beliefs
```

**`strategy/okrs.md`**
```
# OKRs — [Period]
## Objective 1: [outcome]
> Why this matters:
| Key Result | Baseline | Target | Status |

## What We're Deprioritizing
## End-of-Period Retrospective
```

Also fill in these files from the interview answers (overwrite the placeholders):

**`CONSTRAINTS.md`** — fill team, budget, timeline, and non-negotiables from what the human told you

**`CONTEXT.md`** — fill "This Week" and "Next 2 Weeks" based on the goals they stated; leave numbers blank for them to fill

**`AGENT.md`** — compile a fresh brief from all files just created; set "Last updated" to today

Then ask: "Want me to also draft a messaging framework and ICP? Takes a few minutes and means marketing and sales are ready to go."

If yes, create:
- `marketing/messaging-framework.md`
- `sales/icp.md`

Then ask: "Want to fill in your stack and tools? Helps the agent give more grounded advice on PRDs and campaigns."

If yes, fill in `ops/stack.md` with whatever tools the human mentions.

When done: "Your workspace is ready. Every session from now on I'll read this context automatically. Run the weekly ritual every Sunday to keep AGENT.md fresh — paste it into any AI chat for instant context."

---

## DAILY

### Read first (every session, no exceptions)
1. `business-context.md`
2. `CONTEXT.md` — what's actually happening right now
3. `CONSTRAINTS.md` — hard limits on all decisions
4. `strategy/vision.md`
5. `strategy/okrs.md`
6. `DECISIONS.md` — skim last 3–5 entries

If `strategy/vision.md` or `strategy/okrs.md` don't exist: "It looks like setup isn't complete. Want to finish the onboarding now?" Then run the ONBOARDING fill-the-repo steps for the missing files only.

### Opening

Greet with one line on where things stand, then:

> "What do you want to work on today?"
>
> 1. Write a PRD
> 2. Plan a campaign
> 3. Build a sales playbook or outreach sequence
> 4. Design an experiment
> 5. Review or update strategy / OKRs
> 6. Summarize the workspace for a new team member
> 7. Do the weekly ritual (update CONTEXT.md + regenerate AGENT.md)

---

### 1 — Write a PRD

Ask: feature/problem, which OKR it serves, who the user is, any constraints.

Create `product/YYYY-MM-[slug].md`:
```
# PRD: [Feature]
## OKR Alignment: [Objective > Key Result]
## Problem
## Who It's For
## Success Metrics
## Scope (In / Out)
## Requirements
## Open Questions
```

---

### 2 — Plan a Campaign

Ask: which OKR, channel, target audience, timeline, budget.

Create `marketing/YYYY-MM-[slug].md`:
```
# Campaign: [Name]
## OKR Alignment: [Objective > Key Result]
## Goal + Metric + Target
## Audience
## Channel
## Message (Hook / Core message / CTA)
## Timeline
## Results (fill after)
```

---

### 3 — Build a Sales Playbook or Outreach Sequence

Ask: playbook or sequence, which segment, which OKR, what triggers the motion.

Playbook → `sales/playbook-[segment].md`:
```
# Playbook: [Segment]
## OKR Alignment
## Target Segment + Why They Buy
## Entry Point
## Discovery Questions
## Value Pitch
## Objection Responses
## Deal Stages
```

Outreach sequence → `sales/outreach-[segment].md`:
```
# Outreach: [Segment]
## OKR Alignment
## Sequence (Day 0 email / Day 2 LinkedIn / Day 5 follow-up / Day 10 close)
## Each message: Subject + Body + CTA
## Success Metrics
```

---

### 4 — Design an Experiment

Ask: what hypothesis, which OKR it tests, how to measure, sample size and duration.

Create `experiments/YYYY-MM-[slug].md`:
```
# Experiment: [Hypothesis]
## OKR Alignment: [Objective > Key Result]
## Hypothesis: We believe X will cause Y because Z
## Design (control / variant / sample / duration)
## Success Metric + Pass Threshold
## Observations
## Result + Why
## Decision + Learning
```

---

### 5 — Review or Update Strategy / OKRs

Read all files in `strategy/`. Ask what's changed, what's off track, what's new. Propose edits. Show before/after. User confirms before writing.

---

### 6 — Summarize the Workspace

Read the full repo. Write a 5-minute briefing:
- What the business is and who it serves
- Vision and strategic direction
- Active OKRs and status
- What each domain is working on
- Key decisions made and what they ruled out

---

### 7 — Weekly Ritual

Follow `ops/rituals.md`. In sequence:

1. Ask: "What happened last week? What's the focus this week? Any blockers? Current numbers?"
   → Update `CONTEXT.md` with answers.

2. Ask: "Any decisions made this week worth logging?"
   → If yes, append to `DECISIONS.md` using the format in that file.

3. Regenerate `AGENT.md`:
   → Read `business-context.md`, `CONTEXT.md`, `strategy/vision.md`, `strategy/okrs.md`, `CONSTRAINTS.md`, and last 5 entries of `DECISIONS.md`.
   → Rewrite `AGENT.md` as a fresh compiled brief. Update the "Last updated" date.

4. Ask: "Any OKRs to update status on?"
   → If yes, update the status column in `strategy/okrs.md`.

When done: "Ritual complete. AGENT.md is fresh — paste it into any AI chat for instant context."

---

## Rules

- Read the cascade before every domain task
- Every output links to an OKR — if it can't, flag it before proceeding
- Ask the minimum questions; don't ask for what's already in context
- Never overwrite real content without showing the diff first
- Keep all output in Markdown
