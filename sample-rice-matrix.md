# 📊 Full Example — RICE Matrix with NotebookLM Insights

> This is an example of what a real analysis session would look like. Data is illustrative.

---

## Example Context

**Product:** SaaS project management platform
**Feedback analyzed:** 18 PDFs (NPS Q1, 12 interviews, January–March tickets, G2 reviews)
**Monthly active users:** 5,000
**Product team:** 2 PMs, 6 Engineers, 2 Designers

---

## Prompt executed in NotebookLM:
```
"Based on all feedback documents, identify the 8 most frequently mentioned initiatives and give me the inputs to calculate the RICE score for each. Include mention frequency and sources."
```

---

## NotebookLM Output → RICE Inputs

| # | Initiative | Sources | Reach est. | Impact | Confidence | Effort (pm) | **RICE** | Priority |
|---|-----------|---------|-----------|--------|------------|------------|---------|----------|
| 1 | Export reports to Excel | 14/18 docs | 3,500 | 2 | 100% | 1 | **7,000** | 🔥 Critical |
| 2 | Slack notifications | 11/18 docs | 2,800 | 2 | 80% | 2 | **2,240** | 🔥 High |
| 3 | Guided onboarding | 12/18 docs | 4,000 | 3 | 100% | 4 | **3,000** | 🔥 Critical |
| 4 | Bulk task assignment | 8/18 docs | 1,500 | 2 | 80% | 2 | **1,200** | ✅ High |
| 5 | Mobile Kanban view | 9/18 docs | 2,000 | 1 | 80% | 3 | **533** | ✅ Medium |
| 6 | Dark mode | 7/18 docs | 2,500 | 0.5 | 100% | 1 | **1,250** | ✅ Medium |
| 7 | Public documented API | 6/18 docs | 800 | 3 | 50% | 8 | **150** | 🟡 Medium |
| 8 | Jira integration | 5/18 docs | 600 | 2 | 50% | 5 | **120** | ⬇️ Low |

---

## Top 3 Initiative Deep Dives

### 🥇 #1 — Export Reports to Excel (RICE: 7,000)

**NotebookLM insight:**
> "The export problem appears in 14 of 18 documents. In support tickets (January–March) it represents 23% of all requests. In Discovery interviews, 8 of 12 users described manual workarounds (copy-pasting to Excel) as their biggest daily frustration. A representative quote from NPS Q1 (source: NPS-Enterprise-Q1-2025.pdf, response ID-089): 'I need this to report to management every week — without it the product is not viable for us.'"

**Decision:** Immediate sprint. No dependencies.

---

### 🥈 #2 — Guided Onboarding (RICE: 3,000)

**NotebookLM insight:**
> "Mentioned in 12 documents, mostly in interviews with new users (<3 months) and G2 reviews rated 2–3 stars. Clear pattern: users drop off in the first 7 days due to lack of direction. Quote from G2 review (source: Reviews-G2-Q4-2024.pdf): 'Powerful but intimidating. It took me 3 weeks to figure out how to use it properly.'"

**Decision:** Q2 project. Assign 1 designer + 2 engineers.

---

### 🥉 #3 — Slack Notifications (RICE: 2,240)

**NotebookLM insight:**
> "11 documents mention it. Especially frequent in the Enterprise segment (6/6 Enterprise interviews requested it). High confidence (80%) based on robust qualitative evidence and correlation with support tickets about email notifications being 'ignored'."

**Decision:** Parallel Q2 sprint. Integrations team (2 engineers, 3 weeks).

---

## Team Notes

> **PM Note (04/01/2025):** RICE scores were validated with the engineering team on 03/28. The Effort for "Export to Excel" was initially estimated at 2 person-months but engineering reduced it to 1 after identifying a compatible open-source library. This doubled the RICE Score and confirmed it as priority #1.
