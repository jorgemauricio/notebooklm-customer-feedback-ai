# 📄 Guide to Structuring Customer Feedback PDFs

> Before uploading feedback to NotebookLM, make sure your PDFs follow this structure. A well-structured document generates insights up to 3x more accurately.

---

## Why does structure matter?

NotebookLM analyzes the text content of PDFs. Documents with clear structure, labeled sections, and metadata allow the AI to:
- Identify context (who spoke? when? which channel?)
- Efficiently compare feedback across different sources
- Cite the exact section of the document with precision

---

## Recommended Structure by Document Type

### 📋 TYPE 1 — Satisfaction Surveys (NPS, CSAT, CES)
```
COVER / HEADER:
- Study name
- Period: [Q1 2025 / January–March 2025]
- Segment evaluated: [Enterprise / SMB / All]
- Number of responses: [N=245]
- Average score: [NPS: +42]

SECTION 1 — QUANTITATIVE RESULTS
- Score distribution
- Comparison vs. previous period
- Breakdown by category/plan/region

SECTION 2 — QUALITATIVE COMMENTS
Format per response:
[Anonymous ID] | [Score] | [Segment] | [Date]
"Customer's verbatim comment here..."

SECTION 3 — IDENTIFIED THEMES (if available)
- List of tags/categories
- Frequency by theme
```

---

### 🎙️ TYPE 2 — Interview Transcripts
```
HEADER:
- Date: [MM/DD/YYYY]
- Customer type: [Person/Company + Segment]
- Interviewer: [Name or initial]
- Duration: [45 min]
- Goal: [Discovery / Validation / Churn interview]

NOTE: Anonymize customer names — use [Customer A], [Customer B]

TRANSCRIPT:
[Interviewer]: Question here
[Customer A]: Customer's response here

FINDINGS SUMMARY (at the end):
- Pain points mentioned
- Key quotes
- Observed behaviors
- Inferred latent needs
```

---

### 📧 TYPE 3 — Support Tickets / Complaints
```
HEADER:
- Period: [Month/Quarter]
- Total volume: [N tickets]
- Channel: [Email / Chat / Phone / In-app]
- Main category: [Bug / Feature Request / Question / Complaint]

FORMAT PER TICKET (anonymized):
TICKET #[ID] | [Category] | [Priority] | [Resolved: Yes/No]
Customer: [Segment: Enterprise/SMB]
Reported problem: "Problem description as reported by the customer"
Resolution applied: [Description or "Unresolved"]
Resolution time: [X days]

AGGREGATE AT THE END:
- Top 10 most frequent issues
- % of unresolved tickets
- Average resolution time by category
```

---

### 🌐 TYPE 4 — Public Reviews
```
HEADER:
- Platform: [G2 / Capterra / App Store / Play Store]
- Period: [Q1 2025]
- Average rating: [4.2/5]
- Total reviews: [N=89]

FORMAT PER REVIEW:
[Rating: X/5] | [Date] | [User type if available]
Title: "Review title"
"Full review content here..."

ANALYSIS SECTION:
- Most mentioned positive themes
- Most mentioned negative themes
- Competitor comparisons mentioned
```

---

## File Naming Conventions
```
[TYPE]-[SEGMENT]-[PERIOD]-[VERSION].pdf

Examples:
NPS-Enterprise-Q1-2025-v1.pdf
Interviews-SMB-January2025-v2.pdf
Tickets-All-H1-2025-v1.pdf
Reviews-G2-Q4-2024-v1.pdf
```

---

## Checklist Before Uploading to NotebookLM

- [ ] PDF has a header with period and context
- [ ] Customer names are anonymized
- [ ] Qualitative comments are separated into individual entries
- [ ] File name follows the naming convention
- [ ] PDF is text-based (not a scanned image without OCR)
- [ ] Personal data removed (emails, phones, addresses)
