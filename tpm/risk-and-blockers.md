# ⚠️ Risk & Blockers Prompts

**Role:** Technical Project Manager  
**Category:** Risk Management & Blocker Resolution  
**Use when:** Identifying risks early, building a risk register, unblocking teams, or doing a pre-launch review.

---

## Prompt 1 — Risk Register Builder

```
You are a Technical Project Manager building a risk register for a project.

Project name: [e.g., "CRM Integration with Salesforce"]
Project phase: [e.g., planning / development / testing / deployment]
Project summary: [2–3 sentences on what the project does and who it serves]
Team size and roles: [e.g., 3 engineers, 1 QA, 1 PM, external vendor]
Known constraints: [timeline, budget, dependencies, staffing, compliance requirements]

Please generate a risk register with at least 8 risks that includes:
- Risk ID (R-001, R-002, etc.)
- Risk description (clear, specific — not vague)
- Category (Technical / Resource / Timeline / External / Compliance)
- Likelihood (Low / Medium / High)
- Impact (Low / Medium / High)
- Risk score (Likelihood × Impact)
- Mitigation strategy (what we do to reduce the risk)
- Contingency plan (what we do if the risk materializes)
- Owner (role responsible for monitoring this risk)

Format as a table.
```

---

## Prompt 2 — Blocker Triage & Resolution Plan

```
You are a Technical Project Manager helping triage active blockers on a project.

Project: [name]
Current sprint / milestone: [sprint number or milestone name]
Team: [roles involved]

Blockers:
1. [Describe blocker 1 — what it is, how long it's been active, who it impacts]
2. [Describe blocker 2]
3. [Add more as needed]

For each blocker, provide:
1. Root cause analysis (likely reason this is blocked)
2. Severity (Critical / High / Medium — impact on team velocity and timeline)
3. Resolution options (at least 2 paths forward)
4. Recommended action with reasoning
5. Who needs to be involved to unblock it
6. Escalation trigger: "If not resolved by [date], escalate to [role]"

Also provide a summary paragraph I can share in our next standup.
```

---

## Prompt 3 — Pre-Launch Risk Review

```
You are a Technical Project Manager conducting a pre-launch risk review 1–2 weeks before a go-live.

Product / feature launching: [name and brief description]
Launch date: [date]
Launch type: [full rollout / phased rollout / canary / internal only first]
Target users affected: [number and type]
Systems involved: [e.g., backend API, mobile app, third-party payment processor]

Go/No-Go criteria we've defined: [list, or "none yet"]

Please generate:
1. A pre-launch risk checklist (technical, operational, communication, rollback readiness)
2. Top 5 risks specific to this launch with mitigation steps
3. A rollback plan outline: triggers, steps, owner, estimated time to rollback
4. A Go/No-Go decision framework: what conditions mean we launch vs. delay
5. Recommended war room or on-call structure for launch day
```

---

## Prompt 4 — Post-Incident / Retrospective Risk Analysis

```
You are a Technical Project Manager leading a post-incident or post-project retrospective focused on risks.

What happened: [brief description of the incident or project outcome]
Timeline: [when it started, when it was resolved or project ended]
Impact: [customer impact, internal impact, duration, severity]
What was done to resolve it: [steps taken]
What we know about the root cause: [preliminary findings]

Please generate:
1. A blameless root cause analysis (5 Whys format)
2. A list of risk signals that were missed or ignored leading up to this
3. Process improvements to prevent recurrence (with owners and timelines)
4. Metrics to monitor going forward as early warning signals
5. A draft postmortem summary suitable for sharing with leadership
```

---

## Tips for Using These Prompts

- Run Prompt 1 at project kickoff — a risk register started late is half as useful.
- Use Prompt 2 in your weekly syncs to keep blocker resolution moving.
- Prompt 3 is most valuable when combined with your QA lead and a senior engineer in the room.
- Prompt 4 sets the tone for psychological safety — always frame retrospectives as blameless.
