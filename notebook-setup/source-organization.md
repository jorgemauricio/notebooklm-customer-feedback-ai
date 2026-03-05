# 🗂️ Source Organization in NotebookLM

> How you organize sources inside each notebook directly affects the
> quality and precision of the AI's responses. This guide covers
> how to structure, label, and manage sources effectively.

---

## Core Principle: One Objective, One Notebook

Never mix feedback from different objectives in the same notebook.
NotebookLM synthesizes across all active sources simultaneously —
mixing contexts produces vague, unfocused insights.

| ✅ Correct | ❌ Incorrect |
|-----------|-------------|
| Notebook: "NPS Analysis Q1 2025" with only NPS PDFs | Notebook: "All Feedback 2025" with every PDF you have |
| Notebook: "Churn Interviews H1 2025" with exit interviews only | Notebook: "Customer Stuff" mixing tickets, reviews, and interviews |

---

## Recommended Source Sets per Notebook

### 📓 Notebook 1 — General Voice of the Customer
**Goal:** Broad trend analysis, overall sentiment, recurring themes

| Source Type | Files to include |
|-------------|-----------------|
| NPS surveys | All segments, last 2–4 quarters |
| CSAT surveys | All segments, same period |
| Public reviews | G2, Capterra, App Store — last 2 quarters |

**Ideal source count:** 8–15 PDFs
**Refresh cadence:** Quarterly

---

### 📓 Notebook 2 — Discovery & Qualitative Research
**Goal:** Deep understanding of specific problems or user segments

| Source Type | Files to include |
|-------------|-----------------|
| Interview transcripts | Relevant to the feature area being researched |
| Usability session notes | Same feature area |
| Open-ended survey responses | If exported separately as PDFs |

**Ideal source count:** 5–12 PDFs
**Refresh cadence:** Per research sprint

---

### 📓 Notebook 3 — Support Intelligence
**Goal:** Identify recurring bugs, friction points, unmet needs

| Source Type | Files to include |
|-------------|-----------------|
| Support ticket batches | Last 1–2 quarters, grouped by category |
| Bug report summaries | Same period |
| FAQ or help center queries | If available as PDF exports |

**Ideal source count:** 10–20 PDFs
**Refresh cadence:** Monthly

---

### 📓 Notebook 4 — Retention & Churn Analysis
**Goal:** Understand why customers leave or stay

| Source Type | Files to include |
|-------------|-----------------|
| Exit interviews | All churned segments |
| Churn surveys | Same period |
| NPS detractor comments | Exported separately |
| Win/loss interviews | Loss side only |

**Ideal source count:** 6–12 PDFs
**Refresh cadence:** Quarterly

---

### 📓 Notebook 5 — Competitive Intelligence
**Goal:** Surface competitor mentions and benchmark gaps

| Source Type | Files to include |
|-------------|-----------------|
| Win/loss interviews | Both wins and losses |
| Public reviews mentioning competitors | G2, Capterra |
| Churn interviews | Where competitor was cited as reason |
| Sales call notes | If available and anonymized |

**Ideal source count:** 8–15 PDFs
**Refresh cadence:** Quarterly

---

## How to Label Sources Inside NotebookLM

After uploading each PDF, rename it inside NotebookLM for clarity.
The file name you see in the sources panel should be human-readable.

| Uploaded file name | Rename to in NotebookLM |
|-------------------|------------------------|
| `NPS-All-Q1-2025-v1.pdf` | `NPS Survey — All Segments — Q1 2025` |
| `INT-Enterprise-Jan2025-v2.pdf` | `Enterprise Interviews — January 2025` |
| `TICKET-SMB-H1-2025-v1.pdf` | `SMB Support Tickets — H1 2025` |
| `REVIEW-All-Q4-2024-v1.pdf` | `Public Reviews (G2 + Capterra) — Q4 2024` |

> 💡 NotebookLM uses the source label when citing references.
> A clear label like "Enterprise Interviews — January 2025" makes
> citations far more useful than a raw file name like `INT-Enterprise-Jan2025-v2.pdf`.

---

## Managing Sources Over Time

### Adding new sources mid-cycle
- Upload the new PDF and label it immediately
- Re-run any relevant prompts to see if insights shift
- Note the date you added it in the notebook's notes panel

### Deactivating sources for focused queries
- Uncheck sources you want to exclude before running a prompt
- Useful when comparing specific periods (e.g., Q1 vs Q2 only)
- Re-enable all sources after the focused query

### Archiving a notebook
When a planning cycle closes:
1. Export all saved notes from the notebook as a PDF
2. Save the exported summary to your team's shared drive
3. Rename the notebook with an `[ARCHIVED]` prefix
4. Do not delete — it serves as a historical reference

---

## Source Quality Checklist

Before marking a source as ready to use, verify:

- [ ] File follows the naming convention from `naming-conventions.md`
- [ ] PDF is text-based (not a scanned image without OCR)
- [ ] Customer names and personal data are anonymized
- [ ] Document has a clear header with period and segment context
- [ ] File size is under 50MB (NotebookLM limit per source)
- [ ] Content is relevant to this notebook's specific objective

---

## Troubleshooting Common Source Issues

| Problem | Likely cause | Fix |
|---------|-------------|-----|
| NotebookLM can't read the PDF | Scanned image without OCR | Run OCR first using Adobe Acrobat or Google Drive |
| Citations point to wrong section | No section headers in PDF | Add clear section titles to your PDF template |
| AI ignores some sources | Source is deactivated | Check all sources are checked in the panel |
| Responses are too generic | Too many mixed sources | Split into separate notebooks by objective |
| Source upload fails | File over 50MB | Compress or split the PDF into smaller files |
