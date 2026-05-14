# Throughline

**Your business strategy as code. Set it up once, and every AI session — Claude Code, Claude chat, any agent — works from the same context automatically.**

---

Strategy dies in Notion pages nobody reads, slide decks that go stale, and Slack threads nobody finds. Every new hire re-asks the same questions. Every AI session starts from scratch.

Throughline fixes that. Your vision, OKRs, constraints, and decisions live in a git repo — versioned, readable, and inherited by every tool you use.

---

## How It Works

**Set up once (~10 min).** Open in Claude Code. The agent interviews you, does research, and writes your entire foundation — vision, OKRs, constraints, decisions, messaging, ICP.

**Use everywhere.** Every session — Claude Code, Claude chat, any agent — reads the same context. No re-explaining. No drift. Paste `AGENT.md` into any AI for instant context.

**Stay current (15 min/week).** Sunday ritual: update what changed, log decisions, regenerate the agent brief. Done.

---

## The Files

```
AGENT.md          ← Instant AI briefing. Regenerated weekly from the repo state. Do not edit manually.
CONTEXT.md        ← Current reality snapshot. Updated weekly in the Sunday ritual with what shipped, what is happening, and what is blocked.
DECISIONS.md      ← Append-only history of major choices. Each entry explains what was decided, why, what it rules out, and who made it.
CONSTRAINTS.md    ← Hard limits for every decision: team capacity, budget, tech, timeline, and non-negotiables.
business-context.md ← Core business facts captured during onboarding: product, customer, problem, and stage.

strategy/         ← Vision, differentiation, and OKRs. Every product, marketing, sales, and experiment document should trace back here.
product/          ← PRDs and feature plans. Each document should link to a specific OKR and clarify user need.
marketing/        ← Campaign and messaging briefs. Each piece should align to an OKR and a target audience.
sales/            ← Sales playbooks and outreach sequences. Designed for specific segments, triggers, and win criteria.
experiments/      ← Hypothesis-driven tests. Each experiment should have a control, variant, success metric, and learning.

ops/
  stack.md        ← Current operating tools, platforms, and integrations across the business.
  rituals.md      ← The weekly maintenance process that keeps the repo current and AI-friendly.
```

---

## The Rule

Every artifact — PRD, campaign, playbook, experiment — links to an OKR. If it can't, it doesn't get built.

---

## Getting Started

```
1. Fork this repo
2. Open in Claude Code
3. Say: "Let's get started"
```

The agent interviews you, fills the repo, and your brief is ready to share with the whole team — and any AI you use.

---


