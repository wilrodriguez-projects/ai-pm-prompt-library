# 📣 Data Storytelling Prompts

**Role:** Data Analyst  
**Category:** Translating Data into Insights & Narratives  
**Use when:** Presenting findings to stakeholders, writing analysis summaries, turning metrics into decisions, or explaining "so what" behind the numbers.

---

## Prompt 1 — Turn Raw Metrics into a Stakeholder Narrative

```
You are a data analyst helping communicate findings to a non-technical business audience.

Audience: [e.g., VP of Sales / Product team / Customer Success leadership]
Decision or question this data supports: [e.g., "Should we expand the pilot program to more regions?"]

Here are the key metrics:
[Paste your numbers, table, or findings here]

Context:
- Time period covered: [e.g., Q1 2025]
- Comparison period (if any): [e.g., vs. Q4 2024 or vs. same period last year]
- Any important caveats about the data: [e.g., "missing data for 2 weeks in March"]

Please write an analysis narrative that:
1. Opens with the "so what" — the key insight in one sentence
2. Supports it with 2–3 data points that tell the story
3. Acknowledges what the data does NOT tell us
4. Ends with a clear, specific recommendation or next step
5. Is written for someone who won't read past the first paragraph if it's not compelling
```

---

## Prompt 2 — Build an Insight Slide (Slide-Ready Summary)

```
You are a data analyst preparing findings for a presentation slide.

Slide title suggestion: [e.g., "Churn is accelerating in the SMB segment"]
Key data point(s): [paste numbers or findings]
Comparison or trend: [e.g., "Up 12% month-over-month for 3 consecutive months"]
Why this matters to the business: [e.g., "SMB accounts for 35% of ARR"]
What action this should drive: [e.g., "Prioritize retention playbook for accounts < $10K ARR"]

Generate:
1. A punchy slide headline (insight-driven, not "Q1 Metrics Update")
2. Three bullet points of supporting evidence (one idea per bullet, no filler)
3. A "So What" box: the business implication in 1–2 sentences
4. A "Next Step" box: one clear recommended action with an owner role attached
5. Speaker notes: what the presenter should say that the slide doesn't show
```

---

## Prompt 3 — Explain a Metric Movement (Why Did This Number Change?)

```
You are a data analyst investigating an unexpected change in a key metric.

Metric name: [e.g., "Weekly Active Users", "Conversion Rate", "Average Handle Time"]
What changed: [e.g., "Dropped 18% week-over-week" / "Spiked 40% on April 3rd"]
Time period: [e.g., "April 1–7, 2025"]
Affected segment (if known): [e.g., "All users" / "Mobile users only" / "Enterprise tier"]
What we know so far: [any changes deployed, campaigns run, data anomalies noticed]
What we don't know yet: [open questions]

Please:
1. Generate a structured hypothesis list — possible explanations ranked by likelihood
2. For each hypothesis, suggest the SQL query or data check that would confirm or rule it out
3. Write a short "here's what we're seeing" message I can send to stakeholders while investigation is ongoing
4. Suggest what metrics to monitor over the next 7 days to track resolution
```

---

## Prompt 4 — Write an Analysis Summary (Long-Form)

```
You are a data analyst writing a full analysis summary to document findings for the team.

Analysis title: [e.g., "Q1 2025 Customer Retention Analysis"]
Objective: [What question were you trying to answer?]
Data sources used: [list tables, tools, or data exports]
Time period: [date range]
Key findings: [bullet list of what you found]
Anomalies or data quality issues encountered: [describe or "none"]
Limitations: [what this analysis can't tell us]
Recommendations: [what you suggest the team do based on the findings]

Write a structured analysis summary that includes:
1. Executive Summary (3–4 sentences, outcome-focused)
2. Background & Objective
3. Methodology (how the analysis was done, without deep technical jargon)
4. Key Findings (narrative + supporting data)
5. Limitations & Caveats
6. Recommendations
7. Suggested Follow-Up Analyses

Tone: professional, confident, and clear. Avoid hedging language like "it seems" or "possibly might."
```

---

## Tips for Using These Prompts

- The best data story answers "so what?" within the first 30 seconds. Use Prompt 1 to nail that structure.
- Prompt 2 is most useful when you need to hand off findings to someone else who will present them.
- Use Prompt 3 when you're in triage mode — it gives you a clear investigation plan fast.
- Prompt 4 is your go-to for documenting analysis that needs to live in Confluence or Notion for future reference.
