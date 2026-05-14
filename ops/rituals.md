# Weekly Ritual

> Every Sunday. 15 minutes. Keeps the repo — and every AI session — working from reality, not stale context.

---

## Why This Matters

Every AI session reads this repo. If the context is stale, the outputs are stale. 15 minutes on Sunday means every session next week starts sharp.

---

## The Ritual (15 min)

### 1 — Update `CONTEXT.md` (5 min)

Answer honestly:
- What did we actually ship or do last week?
- What are we focused on this week?
- What's blocking us?
- What are the current numbers?
- What's coming in the next 2 weeks?

### 2 — Log decisions in `DECISIONS.md` (3 min)

Any decision made this week that's worth remembering — product, strategy, hiring, pricing, anything. Append to the top. Use the format:

```
## YYYY-MM-DD — [Decision title]
**Decision:** ...
**Why:** ...
**Rules out:** ...
**Who:** ...
```

### 3 — Regenerate `AGENT.md` (2 min)

Open Claude Code and say: **"Regenerate AGENT.md from the current state of the repo."**

The agent reads all core files and rewrites AGENT.md as a fresh compiled brief. Review it. Looks right → done.

### 4 — Check OKR status in `strategy/okrs.md` (5 min)

For each Key Result: update the status column (On track / At risk / Done).

If something is consistently At Risk for 2+ weeks: that's a signal — either the KR is wrong or the work is. Surface it next planning session.

---

## That's It

Commit the changes. Next week, every AI session — Claude Code, Claude chat, or any other agent — starts from a current, accurate picture of the business.

---

## Monthly Add-On (30 min, first Sunday of the month)

- Review `CONSTRAINTS.md` — has anything changed?
- Review `ops/stack.md` — any tool additions or removals?
- Are current OKRs still the right bets, or has something shifted?
