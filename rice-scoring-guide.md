# 📊 RICE Framework Guide for Feedback Prioritization

## What is RICE?

RICE is a prioritization framework created by Intercom's product team. Its name is an acronym for the four factors it evaluates:

| Factor | What it measures | Role |
|--------|-----------------|------|
| **R**each | How many users it impacts | Numerator |
| **I**mpact | How significant the change is | Numerator |
| **C**onfidence | How certain we are | Numerator |
| **E**ffort | How much work it requires | Denominator |

### Formula:
```
RICE Score = (Reach × Impact × Confidence) / Effort
```

**The highest score = highest priority**

---

## How to Score Each Factor

### 🔵 REACH
*How many users does this initiative impact per quarter?*

Use the real or estimated number of affected users:
- If 500 users need it → Reach = 500
- If 30% of your base (e.g., 3,000 users) → Reach = 3,000

> 💡 With NotebookLM feedback, ask: "How many distinct sources/segments mention this problem?"

---

### 🟡 IMPACT
*How much does it move the needle for each affected user?*

Use Intercom's fixed scale:

| Score | Description | When to use |
|-------|-------------|-------------|
| 3 | Massive impact | Resolves a critical blocker; potential to change user behavior |
| 2 | High impact | Significant improvement in experience or conversion |
| 1 | Medium impact | Noticeable improvement but not transformative |
| 0.5 | Low impact | Minor improvement, quality of life |
| 0.25 | Minimal impact | Nice-to-have, barely perceptible |

---

### 🟢 CONFIDENCE
*How certain are we about our Reach and Impact estimates?*

| Percentage | When to use |
|------------|-------------|
| 100% | Solid quantitative data + multiple feedback sources |
| 80% | Robust qualitative feedback + some metrics |
| 50% | Few sources, anecdotal feedback |
| 20% | Intuition or hypothesis with insufficient evidence |

> 🔴 If confidence is below 50%, treat this as a "moonshot" and deprioritize until validated with more data.

---

### 🔴 EFFORT
*How many person-months does this initiative require?*

| Score | Estimated time |
|-------|---------------|
| 0.5 | Less than 2 weeks (1 person) |
| 1 | ~1 month (1–2 people) |
| 2 | 1–2 months as a team |
| 3 | 2–3 months as a team |
| 5+ | Major project (several months, multiple teams) |

---

## Interpreting the Final Score

| RICE Score | Interpretation |
|------------|---------------|
| > 200 | 🔥 Top priority — execute in next sprint/cycle |
| 100–200 | ✅ High priority — next quarter |
| 50–100 | 🟡 Medium priority — qualified backlog |
| < 50 | ⬇️ Low priority — revisit in next planning cycle |

---

## Common Mistakes to Avoid

1. **Inflating Reach** — be conservative. Use active users, not total registered accounts.
2. **Undervaluing Effort** — involve the engineering team to estimate.
3. **Ignoring Confidence** — if you lack data, lower the confidence score, don't skip it.
4. **Comparing initiatives of different types** without adjusting the Reach time period.
5. **Treating RICE as absolute law** — it is a conversation tool, not an oracle.
