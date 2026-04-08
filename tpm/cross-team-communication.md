# 🤝 Cross-Team Communication Prompts

**Role:** Technical Project Manager  
**Category:** Cross-Team & Cross-Functional Communication  
**Use when:** Running meetings, tracking action items, managing handoffs, or aligning teams with different priorities.

---

## Prompt 1 — Meeting Agenda Builder

```
You are a Technical Project Manager preparing a meeting agenda.

Meeting type: [e.g., sprint review / cross-functional sync / architecture review / vendor call]
Meeting goal: [What is the single most important outcome of this meeting?]
Attendees and roles: [e.g., 2 engineers, product manager, QA lead, external vendor]
Duration: [e.g., 45 minutes]
Context / background: [What's the current situation this meeting addresses?]
Pre-work attendees should do: [any prep required, or "none"]

Please generate:
1. A structured agenda with time blocks that fit within [duration]
2. A clear facilitator note for each agenda item (what to drive toward)
3. Parking lot section for out-of-scope topics
4. Suggested decision or outcome for each section
5. A pre-meeting message (Slack or email) I can send to attendees 24 hours before
```

---

## Prompt 2 — Action Item Tracker & Follow-Up Message

```
You are a Technical Project Manager following up after a cross-team meeting.

Meeting name: [e.g., "Q2 Roadmap Alignment — April 9"]
Attendees: [list names or roles]
Key decisions made: [list]
Raw action items discussed: [paste unformatted notes or bullet points here]

Please:
1. Organize the action items into a clean table with: Action | Owner | Due Date | Priority | Status
2. Flag any action items that are missing an owner or due date
3. Write a follow-up message (Slack or email) summarizing decisions made and action items assigned
4. Identify any open questions that still need an answer before the team can move forward
```

---

## Prompt 3 — Handoff Documentation

```
You are a Technical Project Manager creating a handoff document for work being transitioned between teams, vendors, or sprints.

What is being handed off: [feature, project phase, system, or workstream]
Handing off from: [team or person]
Handing off to: [team or person]
Handoff date: [date]
Current state of the work: [what's done, what's in progress, what's not started]
Known issues or technical debt: [list]
Key contacts for questions: [names/roles]
Critical context the receiving team needs: [business logic, edge cases, decisions made]
Documentation available: [Confluence page, Jira board, GitHub repo, etc.]

Generate:
1. A structured handoff document (clear, not a wall of text)
2. A "first week checklist" for the receiving team
3. A list of open questions the handoff owner should answer before or during the transition
4. A suggested check-in schedule for the first 2–4 weeks post-handoff
```

---

## Prompt 4 — Conflict or Misalignment Resolution Message

```
You are a Technical Project Manager helping navigate a disagreement or misalignment between two teams or stakeholders.

Teams or parties involved: [e.g., engineering team and product team / two engineering teams]
What they disagree on: [scope, priority, technical approach, timeline, resource allocation]
Each side's position:
- Team/Party A: [their view and reasoning]
- Team/Party B: [their view and reasoning]
What's at stake if unresolved: [project impact, relationship impact]
Your role in this: [neutral facilitator / you have a preference / you need a decision fast]

Please generate:
1. An objective summary of the disagreement (useful for bringing in a decision-maker)
2. Areas of common ground between the two sides
3. Two or three resolution options with trade-offs
4. A recommended path forward with rationale
5. A message you can send to both parties to re-align without taking sides
```

---

## Tips for Using These Prompts

- Prompt 1: Send the pre-meeting note the day before — it dramatically reduces meeting sprawl.
- Prompt 2: Run this within 2 hours of a meeting ending while context is fresh.
- Prompt 3: Never hand off undocumented work. Use this prompt to force the structure.
- Prompt 4: Use "two sides" framing when writing to leadership — it signals fairness and analytical thinking.
