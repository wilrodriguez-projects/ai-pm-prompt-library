# 🗂️ Sprint Planning Prompts

**Role:** Technical Project Manager  
**Category:** Sprint & Project Planning  
**Use when:** Kicking off a sprint, scoping work, breaking down epics, or setting team goals.

---

## Prompt 1 — Sprint Kickoff Brief

```
You are a Technical Project Manager. I need to kick off a new sprint.

Here is the context:
- Sprint number / name: [e.g., Sprint 14]
- Sprint duration: [e.g., 2 weeks, starting [date]]
- Team size: [e.g., 4 engineers, 1 QA, 1 designer]
- High-level goals for this sprint: [e.g., complete user authentication flow, fix top 3 production bugs]
- Any carryover from last sprint: [list items or "none"]
- Known dependencies or blockers: [list or "none"]

Please generate:
1. A sprint goal statement (1–2 sentences, outcome-focused)
2. A prioritized list of focus areas (P0 = must ship, P1 = should ship, P2 = stretch)
3. A list of risks or open questions the team should address at kickoff
4. A suggested agenda for the sprint planning meeting (30–60 min)
```

---

## Prompt 2 — Epic Breakdown into Tickets

```
You are a Technical Project Manager helping break down a large feature into sprint-ready work items.

Epic name: [e.g., "Customer Onboarding Redesign"]
Epic goal: [What problem does this solve and for whom?]
Tech stack / context: [e.g., React frontend, Node.js backend, PostgreSQL]
Team involved: [e.g., 2 frontend engineers, 1 backend engineer]
Target completion: [e.g., end of Q2]

Please break this epic into:
1. User stories (written as: "As a [user], I want [action] so that [value]")
2. Engineering tasks per story (specific, actionable, estimable in points or hours)
3. Acceptance criteria for each story
4. Dependencies between tasks
5. Suggested sprint distribution if the epic spans multiple sprints
```

---

## Prompt 3 — Scope Definition & Trade-off Analysis

```
You are a Technical Project Manager. A stakeholder wants to add scope to an in-flight sprint or project.

Current sprint/project state: [e.g., 60% complete, Sprint 12 of 14]
What they want to add: [describe the new request]
Reason given: [their justification]
Team capacity remaining: [e.g., ~20 story points left, 3 engineers for 1 more week]

Please provide:
1. An honest assessment of whether this fits in scope
2. A trade-off analysis: what would need to be cut or delayed to accommodate this
3. A recommended response to the stakeholder (professional, data-driven, not just "no")
4. A revised scope option if a compromise is possible
```

---

## Prompt 4 — Sprint Retrospective Summary

```
You are a Technical Project Manager facilitating a sprint retrospective.

Sprint name/number: [e.g., Sprint 14]
What went well: [bullet list of team input]
What didn't go well: [bullet list of team input]
Action items suggested: [list or "none yet"]
Team mood/energy: [e.g., "a bit tired", "energized", "frustrated with blockers"]

Please generate:
1. A clean retrospective summary suitable for sharing with leadership
2. Top 3 actionable improvements with an owner and a target sprint to resolve
3. A morale note — acknowledge the team's effort without being generic
4. Any process risks to flag before the next sprint starts
```

---

## Tips for Using These Prompts

- Fill in every `[bracketed]` field before submitting — specificity drives quality output.
- These prompts work best in Claude, ChatGPT (GPT-4), or Gemini Advanced.
- Combine Prompt 2 + Prompt 3 when negotiating scope with PMs or stakeholders.
- Save your outputs as sprint artifacts in Confluence, Notion, or Jira descriptions.
