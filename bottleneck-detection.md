# 🔴 Prompt — Bottleneck Detection

> Use this prompt to identify the main friction points, drop-off moments, or blockers in the user experience.

---

## BOTTLENECK DETECTION PROMPT
```
Analyze all loaded feedback documents and detect the main bottlenecks in the user experience.

For each bottleneck found, provide:

1. **PROBLEM NAME** — Short, descriptive title
2. **DESCRIPTION** — What is failing exactly
3. **USER IMPACT** — How it affects their workflow or experience
4. **FREQUENCY** — How many documents/sources mention it (e.g., 8/15 sources)
5. **SEVERITY** — 🔴 Critical / 🟡 Moderate / 🟢 Minor
6. **TIME PATTERN** — Is it recurring? Has it worsened over time?
7. **REPRESENTATIVE QUOTE** — A direct phrase from the feedback that exemplifies it
8. **SOURCES** — List of documents where this issue appears

At the end, generate a summary table ordered by: Frequency × Severity (highest to lowest).

Limit the analysis to the 10 most significant bottlenecks. If there are more, indicate it.
```

---

## Prompt Variations

### For a specific area:
```
[Same prompt above] + "Focus the analysis only on the [onboarding / checkout / support / initial setup] stage"
```

### For a specific customer segment:
```
[Same prompt above] + "Only consider feedback from the [Enterprise / SMB / B2C / new users] segment"
```

### For a specific time period:
```
[Same prompt above] + "Prioritize feedback documents from the [Q1 2025 / last 6 months / post v2.0 launch] period"
```
