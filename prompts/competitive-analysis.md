# 🏆 Prompt — Competitive Analysis from the Voice of the Customer

> Use this prompt to extract competitive intelligence hidden inside your customer feedback.
> Customers often mention competitors, make comparisons, or describe features they've seen
> elsewhere — this prompt surfaces all of that systematically.

---

## WHEN TO USE THIS PROMPT

- Before a quarterly roadmap planning session
- When entering a new market segment
- After a spike in churn that may be competitor-related
- When you need to justify a feature investment to stakeholders
- During win/loss analysis cycles

---

## PROMPT 1 — Competitor Mentions & Comparisons
```
Analyze all loaded feedback documents and extract every instance where customers
mention, compare, or reference competing products or alternative solutions.

For each competitor or alternative mentioned, provide:

1. **COMPETITOR NAME** — Product, tool, or alternative mentioned
   (include generic alternatives like "Excel", "manual process", "the old system")

2. **CONTEXT OF MENTION** — Why is the customer bringing it up?
   - Switching from this competitor to us
   - Switching from us to this competitor
   - Feature comparison ("competitor X does this better")
   - Pricing comparison
   - Considering as an alternative

3. **SENTIMENT** — Positive / Negative / Neutral toward the competitor

4. **FEATURE OR CAPABILITY REFERENCED** — What specific capability is being
   compared or praised in the competitor?

5. **FREQUENCY** — How many sources mention this competitor? (X/Y documents)

6. **REPRESENTATIVE QUOTE** — Direct customer phrase illustrating the comparison

7. **SOURCE** — Document(s) where this appears

At the end, generate a Competitive Mentions Summary Table ordered by frequency.
```

---

## PROMPT 2 — Competitive Gap Analysis
```
Based on all feedback documents, identify the gaps in our product that customers
are explicitly or implicitly attributing to competitor advantages.

For each gap identified, provide:

1. **GAP NAME** — Short descriptive title

2. **DESCRIPTION** — What capability or experience is missing compared
   to what customers expect or have seen elsewhere

3. **COMPETITOR ADVANTAGE** — Which competitor(s) are associated with
   this gap (if named by customers)

4. **CUSTOMER IMPACT** — How is this gap affecting customer behavior?
   Choose one:
   - 🔴 Causing churn or loss of deals
   - 🟡 Creating hesitation or friction in adoption
   - 🟢 Reducing delight but not causing abandonment

5. **FREQUENCY** — How many sources mention this gap? (X/Y documents)

6. **SEGMENT AFFECTED** — Is this gap more critical for a specific
   customer segment? (Enterprise / SMB / specific use case)

7. **SOURCES** — List of reference documents

At the end, rank the gaps from most to least strategically urgent,
and flag which ones represent a risk to retention vs. a risk to acquisition.
```

---

## PROMPT 3 — Win/Loss Patterns
```
Analyze the feedback documents for patterns that explain why customers
chose us over competitors (wins) or chose competitors over us (losses).

## WINS — Why customers chose us:
- What specific reasons do customers give for selecting our product?
- Which features or qualities are most frequently cited as differentiators?
- Are there segments where we win more consistently? Why?

## LOSSES & CHURN — Why customers left or considered leaving:
- What reasons do customers give for switching or considering alternatives?
- Which competitor capabilities are most frequently cited as the reason to leave?
- Are there specific segments where we lose more often?

## PATTERNS TO SURFACE:
- Top 3 reasons we win
- Top 3 reasons we lose
- Any surprising or counterintuitive findings
- Segments where our win rate appears strongest vs. weakest

For each finding, include frequency of mention and at least one
representative quote with its source document.
```

---

## PROMPT 4 — Feature Benchmarking from Customer Language
```
Customers often describe competitor features without naming the competitor.
Analyze all feedback documents and identify instances where customers describe
a capability using phrases like:

- "I wish this worked like..."
- "In my previous tool..."
- "Other platforms do this by..."
- "I used to be able to..."
- "I've seen this done better elsewhere..."

For each instance found:

1. **CUSTOMER DESCRIPTION** — What capability are they describing?
2. **INFERRED BENCHMARK** — What product or standard are they likely
   comparing against? (even if not named)
3. **OUR CURRENT STATE** — Does this capability exist partially,
   fully, or not at all in our product?
   - ✅ Exists fully
   - 🟡 Exists partially
   - ❌ Does not exist
4. **FREQUENCY** — How many customers describe something similar?
5. **SOURCE** — Reference documents

At the end, generate a Feature Benchmark Table showing our coverage
vs. implied market expectations.
```

---

## OUTPUT TEMPLATE — Competitive Landscape Summary

Use this template to document and share findings with your team after
running the prompts above:
```markdown
## Competitive Landscape — [Product Name] — [Period]
**Source:** NotebookLM analysis of [N] feedback documents
**Date:** [MM/DD/YYYY]
**PM Owner:** [Name]

### Competitors Mentioned by Customers
| Competitor | Times Mentioned | Primary Context | Sentiment |
|-----------|----------------|-----------------|-----------|
| | | | |

### Top Competitive Gaps (ranked by urgency)
| # | Gap | Competitor Advantage | Impact | Segment | RICE Candidate? |
|---|-----|---------------------|--------|---------|----------------|
| | | | | | |

### Win Reasons (Top 3)
1.
2.
3.

### Loss Reasons (Top 3)
1.
2.
3.

### Strategic Recommendations
- **Defend:** [What we must protect to retain current customers]
- **Attack:** [Where we can close the gap to win new deals]
- **Ignore:** [Competitor strengths that don't affect our target segment]
```

---

## Tips for Best Results

> 💡 **Load the right sources** — This prompt works best with notebooks
> that contain exit interviews, churn surveys, win/loss notes, and public
> reviews (G2, Capterra). Support tickets rarely contain competitor mentions.

> 💡 **Run Prompt 1 first** — Always start with the competitor mentions
> scan before running gap analysis. It gives you the vocabulary customers
> use, which makes the gap analysis more precise.

> 💡 **Combine with RICE** — Every gap identified in Prompt 2 is a
> candidate for the RICE matrix. Use the `improvement-opportunities.md`
> RICE input prompt immediately after to score them.

> 💡 **Revisit quarterly** — Competitive dynamics shift. Re-run this
> prompt each quarter with updated feedback to track whether gaps are
> growing or shrinking in customer perception.
