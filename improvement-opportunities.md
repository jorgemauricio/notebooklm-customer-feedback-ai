# 🟢 Prompt — Improvements & New Proposals

> Use this prompt to uncover unmet needs, requested features, and areas for competitive differentiation.

---

## IMPROVEMENTS & PROPOSALS PROMPT
```
Analyze all feedback documents and extract improvement opportunities and new feature proposals requested by customers.

Organize findings into three categories:

## CATEGORY 1: IMPROVEMENTS TO EXISTING FEATURES
Current functionality that needs optimization.
For each include:
- Which feature needs improvement
- What users specifically expect
- How frequently it is mentioned (X/Y documents)
- Representative quote + source

## CATEGORY 2: NEW FEATURES REQUESTED
Capabilities that users explicitly ask for that do not yet exist.
For each include:
- Tentative feature name
- The need it solves (Jobs-to-be-Done)
- User segment requesting it
- Frequency of mention + sources

## CATEGORY 3: LATENT INSIGHTS (not explicitly requested, but implied)
Needs that users do not directly articulate, but which are inferred from their frustrations or workarounds.
For each include:
- The workaround or behavior the user describes
- The underlying need it reveals
- Implicit product opportunity
- Reference sources

At the end, generate a ranking of the TOP 5 opportunities with the highest potential based on frequency × perceived impact in the feedback.
```

---

## ROADMAP PRIORITIZATION PROMPT
```
Based on all feedback documents, help me build inputs for the RICE framework.

For the 10 most frequently mentioned or requested initiatives, estimate:

1. **REACH**: What percentage of the user base does it affect? Is it mentioned by users from different segments or just one?
2. **IMPACT**: Based on the tone and urgency of the feedback, what is the expected impact? (Scale: Minimal=0.25, Low=0.5, Medium=1, High=2, Massive=3)
3. **CONFIDENCE**: How much evidence exists in the documents? (High=100%, Medium=80%, Low=50%, Very Low=20%)
4. **EFFORT NOTES**: Are there clues in the feedback about how complex the problem is? (user-perceived complexity)

Present results in a table format ready to bring into the RICE Matrix.
```
