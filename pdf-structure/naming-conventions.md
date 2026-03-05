# 📝 File Naming Conventions

> Consistent naming is critical for NotebookLM to organize and distinguish
> sources correctly. Follow these conventions before uploading any PDF.

---

## Master Naming Formula
```
[TYPE]-[SEGMENT]-[PERIOD]-[VERSION].pdf
```

Every file name has exactly **4 components**, separated by hyphens.
No spaces. No special characters. Always lowercase except for acronyms.

---

## Component Breakdown

### Component 1 — TYPE
What kind of feedback document is this?

| Code | Full Name | Example |
|------|-----------|---------|
| `NPS` | Net Promoter Score survey | `NPS-...` |
| `CSAT` | Customer Satisfaction survey | `CSAT-...` |
| `CES` | Customer Effort Score survey | `CES-...` |
| `INT` | Customer interview transcript | `INT-...` |
| `TICKET` | Support tickets batch | `TICKET-...` |
| `REVIEW` | Public reviews (G2, Capterra, etc.) | `REVIEW-...` |
| `CHURN` | Exit interview or churn survey | `CHURN-...` |
| `WINLOSS` | Win/loss interview | `WINLOSS-...` |
| `ONSITE` | Usability or on-site research session | `ONSITE-...` |
| `SOCIAL` | Social media feedback batch | `SOCIAL-...` |

---

### Component 2 — SEGMENT
Which customer segment does this feedback represent?

| Code | Segment |
|------|---------|
| `All` | All segments combined |
| `Enterprise` | Enterprise accounts |
| `SMB` | Small and medium businesses |
| `B2C` | Individual / consumer users |
| `New` | New users (< 3 months) |
| `Power` | Power users or champions |
| `Churned` | Former customers |
| `Trial` | Trial or freemium users |

---

### Component 3 — PERIOD
What time period does this feedback cover?

| Format | When to use | Example |
|--------|-------------|---------|
| `Q1-2025` | Full quarter | `NPS-All-Q1-2025-v1.pdf` |
| `H1-2025` | Half year | `TICKET-Enterprise-H1-2025-v1.pdf` |
| `Jan2025` | Single month | `INT-SMB-Jan2025-v1.pdf` |
| `2025` | Full year | `REVIEW-All-2025-v1.pdf` |

---

### Component 4 — VERSION
Track iterations of the same document.

| Code | When to use |
|------|-------------|
| `v1` | First upload of this document |
| `v2` | Updated or corrected version |
| `v3+` | Subsequent revisions |

> 💡 Always increment the version rather than overwriting.
> Keep old versions locally for audit purposes even if not uploaded to NotebookLM.

---

## Full Naming Examples

| File Name | What it contains |
|-----------|-----------------|
| `NPS-All-Q1-2025-v1.pdf` | NPS survey, all segments, Q1 2025, first version |
| `INT-Enterprise-Jan2025-v2.pdf` | Enterprise interviews, January 2025, second revision |
| `TICKET-SMB-H1-2025-v1.pdf` | SMB support tickets, first half of 2025 |
| `REVIEW-All-Q4-2024-v1.pdf` | Public reviews from all platforms, Q4 2024 |
| `CHURN-Enterprise-Q2-2025-v1.pdf` | Enterprise exit interviews, Q2 2025 |
| `WINLOSS-All-Q1-2025-v1.pdf` | Win/loss interviews, Q1 2025 |
| `CSAT-B2C-Mar2025-v1.pdf` | B2C CSAT survey, March 2025 |

---

## Anti-patterns to Avoid

| ❌ Bad | ✅ Good | Why |
|--------|---------|-----|
| `customer feedback march.pdf` | `NPS-All-Mar2025-v1.pdf` | Spaces break file paths |
| `NPS_Q1_2025.pdf` | `NPS-All-Q1-2025-v1.pdf` | Missing segment and version |
| `final_final_v3_REAL.pdf` | `INT-SMB-Q1-2025-v3.pdf` | Unclear type and period |
| `feedback(2).pdf` | `TICKET-Enterprise-Feb2025-v2.pdf` | Parentheses cause errors |
| `NPS-enterprise-q1-2025.pdf` | `NPS-Enterprise-Q1-2025-v1.pdf` | Inconsistent capitalization |

---

## Batch Renaming Tips

**On macOS:**
Use Automator or the built-in Finder batch rename (select files → right-click → Rename).

**On Windows:**
Use PowerToys PowerRename for regex-based batch renaming.

**With Python** (if you have many files to rename):
```python
import os

# Example: add version suffix to all PDFs in a folder
folder = "/your/feedback/folder"
for filename in os.listdir(folder):
    if filename.endswith(".pdf") and "-v" not in filename:
        new_name = filename.replace(".pdf", "-v1.pdf")
        os.rename(
            os.path.join(folder, filename),
            os.path.join(folder, new_name)
        )
```
