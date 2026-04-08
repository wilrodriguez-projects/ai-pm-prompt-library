# 🔗 Cross-Program Dependencies Prompts

**Role:** Technical Program Manager  
**Category:** Dependency Management & Program Coordination  
**Use when:** Managing work across multiple teams, tracking inter-program dependencies, coordinating shared resources, or preventing delivery failures caused by untracked handoffs.

---

## Prompt 1 — Dependency Mapping

```
You are a Technical Program Manager mapping dependencies across a portfolio of projects.

Programs / projects in scope:
1. [Project A] — Team: [team name] — Phase: [current phase] — Key deliverable: [what they produce]
2. [Project B] — Team: [team name] — Phase: [current phase] — Key deliverable: [what they produce]
3. [Add more as needed]

Known dependencies (describe what you already know):
- [e.g., "Project B cannot begin testing until Project A delivers the API contract"]
- [e.g., "Project C and Project A share the same QA team"]

Timeline: [overall program window]

Please generate:
1. A dependency matrix (table format): which project depends on what, from whom, by when
2. Critical path narrative: which dependency chain has the least slack and why
3. Top 3 dependency risks (what breaks if a dependency is late)
4. Mitigation suggestions for the riskiest dependencies
5. A dependency tracking cadence recommendation: how often should these be reviewed and with whom
```

---

## Prompt 2 — Dependency Risk Escalation

```
You are a Technical Program Manager escalating a dependency that is at risk of breaking.

Dependency description: [what is supposed to be delivered, by whom, by when]
Receiving team: [who is waiting on this]
Impact if late: [what breaks downstream — timeline, quality, customer impact]
Current status: [how late or at-risk is the delivery?]
Root cause (if known): [why is this at risk?]
What has already been tried: [list attempts to resolve]
What you need: [a decision / resource / priority shift / leadership pressure]

Please write:
1. An escalation message to send to both the delivering and receiving team's leadership
2. Two resolution options with trade-offs
3. A contingency plan if the dependency cannot be resolved in time
4. A decision request: what does leadership need to decide, and by when
```

---

## Prompt 3 — Inter-Team Alignment Meeting Prep

```
You are a Technical Program Manager preparing for a cross-team alignment meeting focused on shared dependencies.

Teams attending: [list]
Meeting goal: [what must be decided or aligned by the end of this meeting]
Background context: [what's the current situation causing the need for alignment?]

Current points of misalignment:
1. [Issue 1: what each team believes or wants]
2. [Issue 2: ...]

Constraints each team is working within:
- [Team A]: [their constraints]
- [Team B]: [their constraints]

Please generate:
1. A structured meeting agenda (45–60 min)
2. Pre-read summary for attendees (context without bias toward either team)
3. Decision framework: what criteria should drive the alignment decision?
4. Likely sticking points and how to facilitate through them
5. A post-meeting communication template to confirm what was decided
```

---

## Prompt 4 — Shared Resource Conflict Resolution

```
You are a Technical Program Manager resolving a conflict over shared resources between two programs.

Shared resource in question: [e.g., "QA team", "DevOps engineer", "staging environment", "budget pool"]
Program A's need: [what they need, when, and why it's urgent]
Program B's need: [what they need, when, and why it's urgent]
Available capacity of the shared resource: [what's actually available]
Priority context: [is one program higher priority? is there a hard customer deadline?]
Current state: [is the conflict active right now, or about to happen?]

Please generate:
1. An objective summary of the conflict (no favoritism)
2. Three resolution options with trade-offs for each program
3. A recommended resolution with clear rationale
4. A communication plan: how to tell both teams what was decided without creating resentment
5. A longer-term recommendation to prevent this type of conflict from recurring
```

---

## Tips for Using These Prompts

- Dependency mapping (Prompt 1) should happen at program kickoff and be reviewed every 2 weeks — not just when something breaks.
- The best dependency escalations (Prompt 2) come with a recommendation attached. Don't just surface a problem — bring options.
- Prompt 3 is most effective when the pre-read is sent 24 hours in advance. Surprises in alignment meetings extend them by 30 minutes minimum.
- Shared resource conflicts (Prompt 4) are where TPgMs earn their reputation. Whoever handles these calmly and fairly becomes the person teams trust.
