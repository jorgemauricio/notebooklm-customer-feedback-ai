# 🗃️ RICE Matrix Template

> Copy this table into Notion, Google Sheets, or any management tool. Scores calculate automatically if you use the formula.

---

## RICE MATRIX — [Product Name / Planning Cycle]
**Analysis period:** [Q1 2025 / H1 2025]
**Data source:** Customer Feedback — NotebookLM Analysis
**Last updated:** [MM/DD/YYYY]
**Owner:** [PM Name]

---

## Main Table

| # | Initiative | Category | Reach | Impact | Confidence | Effort | **RICE Score** | Priority | Status |
|---|-----------|----------|-------|--------|------------|--------|----------------|----------|--------|
| 1 | [Initiative name] | Bug / Feature / UX / Infra | 1000 | 2 | 0.8 | 2 | **800** | 🔥 High | To evaluate |
| 2 | | | | | | | | | |
| 3 | | | | | | | | | |
| 4 | | | | | | | | | |
| 5 | | | | | | | | | |
| 6 | | | | | | | | | |
| 7 | | | | | | | | | |
| 8 | | | | | | | | | |
| 9 | | | | | | | | | |
| 10 | | | | | | | | | |

**Formula:** `RICE Score = (Reach × Impact × Confidence) / Effort`

---

## Initiative Detail Card

### Initiative #1: [Name]

| Field | Value |
|-------|-------|
| **Description** | What it is and what problem it solves |
| **Origin insight** | NotebookLM prompt/analysis that detected it |
| **Feedback sources** | List of PDFs where it is mentioned |
| **Feedback frequency** | X of Y documents mention it |
| **Reach** | [Number] — justification |
| **Impact** | [0.25 / 0.5 / 1 / 2 / 3] — justification |
| **Confidence** | [20% / 50% / 80% / 100%] — justification |
| **Effort** | [person-months] — estimated with engineering |
| **RICE Score** | **(Reach × Impact × Confidence) / Effort** |
| **Dependencies** | Does it block or get blocked by another initiative? |
| **Risks** | Technical or business risks identified |
| **Next step** | Discovery / Prototype / Tech estimation / Sprint |

---

## Quadrant View (for stakeholder presentations)
```
HIGH IMPACT ↑
              |
  🔥 CRITICAL |  ⭐ STRATEGIC
  (do now)    |  (plan carefully)
              |
--------------+---------------- EFFORT →
              |
  ✅ QUICK    |  ⚠️ QUESTIONABLE
  (quick wins)|  (avoid or rethink)
              |
LOW IMPACT ↓
```

| Quadrant | Description | Recommended action |
|----------|-------------|-------------------|
| 🔥 Critical | High impact, low effort | Prioritize immediately |
| ⭐ Strategic | High impact, high effort | Plan with dedicated resources |
| ✅ Quick Wins | Low impact, low effort | Ship between sprints |
| ⚠️ Questionable | Low impact, high effort | Discard or reduce scope |

---

## Change Log

| Date | Initiative | Change | Reason |
|------|-----------|--------|--------|
| | | | |
