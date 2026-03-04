# ⚙️ Notebook Configuration in NotebookLM

---

## Recommended Notebook Architecture

Don't load everything into a single notebook. Follow this structure:
```
📚 NOTEBOOK 1 — "General Feedback [Product] Q1 2025"
   Sources: NPS + Surveys + Public Reviews
   Use: General trend analysis, global voice of the customer

📚 NOTEBOOK 2 — "Discovery Interviews [Feature Area]"
   Sources: Relevant interview transcripts
   Use: Deep-dive into a specific problem or area

📚 NOTEBOOK 3 — "Support Tickets [Q1 2025]"
   Sources: PDFs of tickets grouped by category
   Use: Detect critical bugs, support patterns

📚 NOTEBOOK 4 — "Churn & Retention Feedback"
   Sources: Exit interviews, churn surveys, NPS detractors
   Use: Understand why customers leave

📚 NOTEBOOK 5 — "Competitive Analysis from the Voice of the Customer"
   Sources: Reviews mentioning competitors, win/loss interviews
   Use: Identify competitive gaps as perceived by users
```

> 💡 **Golden rule:** One notebook = One analysis objective. Don't mix contexts.

---

## Step by Step: Creating Your First Notebook

### 1. Access NotebookLM
- Go to [notebooklm.google.com](https://notebooklm.google.com)
- Sign in with your Google account

### 2. Create a new notebook
- Click **"New notebook"**
- Name it with the convention: `[Product] — [Feedback Type] — [Period]`
- Example: `"Mobile App — NPS + Surveys — Q1 2025"`

### 3. Upload sources
- Click **"+ Add source"**
- Upload your prepared PDFs (max 50 sources per notebook)
- Wait for NotebookLM to process each document (1–3 min per PDF)

### 4. Configure notebook instructions
- Click the **pencil / instructions** icon
- Paste the [Master Prompt](../prompts/master-prompt.md)
- Save

### 5. Verify sources are active
- In the side panel, make sure all PDFs have ✓ enabled
- You can select/deselect sources per query

---

## Source Management

| Action | When to do it |
|--------|--------------|
| Add new sources | At the end of each feedback collection sprint |
| Deactivate old sources | When doing analysis for specific time periods |
| Create a new notebook | When the analysis objective or period changes |
| Archive a notebook | When closing a planning cycle |

---

## Technical Limits (Free Version)

| Resource | Limit |
|----------|-------|
| Sources per notebook | 50 documents |
| Words per document | 500,000 words |
| Total notebooks | No known limit |
| Notebook instructions | 10,000 characters |

> For teams with higher volume, consider **NotebookLM Plus** (~$20/user/month via Google One AI Premium).

---

## Advanced Usage Tips

**🎯 Source selection per query:**
To compare Q1 vs Q2, select only the relevant documents before asking your question.

**📝 Save insights as notes:**
When NotebookLM generates a valuable insight, save it as a note inside the notebook (bookmark button). These notes are also queryable.

**🎙️ Audio Overview:**
Generate an audio summary (podcast format) of the notebook to listen to general trends while on the go.

**📊 Data Tables (NotebookLM Plus):**
Export analyses directly to Google Sheets to complement the RICE Matrix.

## 🗺️ End-to-End Workflow

Use this as a final checklist to confirm your notebook is fully configured and ready for analysis.
```
  STEP 1 — PREPARE                    STEP 2 — LOAD
  ──────────────────                  ──────────────────────────
  📄 Structure PDFs            ──▶    📚 Upload to NotebookLM
     · Add headers                       · Max 50 sources
     · Anonymize names                   · 1 notebook per goal
     · Follow naming convention          · Wait for processing

  STEP 3 — CONFIGURE                  STEP 4 — ANALYZE
  ──────────────────────────          ──────────────────────────
  🧠 Paste Master Prompt       ──▶    🔍 Run specialized prompts
     · Notebook Instructions              · Bottleneck detection
     · Sets AI behavior                   · Improvement opportunities
     · Save before querying               · RICE input generation

  STEP 5 — PRIORITIZE                 STEP 6 — DECIDE
  ──────────────────────────          ──────────────────────────
  📊 Fill RICE Matrix          ──▶    🚀 Build your roadmap
     · Score each initiative              · Sprint planning
     · Validate effort with eng.          · Stakeholder presentation
     · Apply quadrant view                · Log decisions & changes
```

> ✅ If you have completed all 6 steps, your NotebookLM system is fully operational.
> Return to [README.md](../README.md) for a full project overview.
