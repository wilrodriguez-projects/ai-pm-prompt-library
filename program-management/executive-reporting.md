# 📋 Executive Reporting Prompts

**Role:** Technical Program Manager  
**Category:** Executive & Leadership Communication  
**Use when:** Preparing board updates, writing QBRs, presenting to C-suite, building leadership dashboards, or summarizing complex programs in limited time and space.

---

## Prompt 1 — Quarterly Business Review (QBR) Narrative

```
You are a Technical Program Manager preparing a QBR presentation for senior leadership.

Quarter being reviewed: [e.g., Q1 2025]
Audience: [e.g., VP Engineering, CTO, Head of Product]
Program or team: [name and brief description]
Planned goals for the quarter: [list OKRs or commitments]
Actual results: [what was delivered — be specific with numbers]
Budget: [planned vs. actual spend]
Headcount/capacity: [planned vs. actual]
Top 3 wins: [specific, quantifiable if possible]
Top 2 misses and why: [honest, blameless assessment]
Key risks heading into next quarter: [list]
Asks from leadership: [what you need — budget, headcount, decisions, air cover]

Please generate:
1. A QBR executive narrative (750 words max, structured for a 10-minute slot)
2. A "scorecard" section: planned vs. actual for the top 5 commitments
3. A concise "look ahead" for next quarter (goals + known risks)
4. Slide headline suggestions for each major section
5. Anticipated tough questions from leadership — and how to answer them
```

---

### 📄 Example Output

**Prompt used:** Q1 QBR — Network Operations Program

---

**Executive Narrative**

Q1 was a quarter of strong execution with one significant external variable we're actively managing heading into Q2.

We delivered on 4 of 5 committed milestones: the NOC dashboard launched on March 28, carrier cutover for the Bedford site completed 3 days ahead of schedule, and our P1 incident rate dropped 31% versus Q4 — the largest single-quarter improvement in 18 months. Runbook coverage reached 78%, up from 55% at the start of the quarter.

The miss: VoIP migration Phase 2 UAT did not begin as planned. A vendor hardware delay pushed lab readiness by 3 weeks. We've identified an alternate provisioning path and UAT is now targeted for April 21. No customer impact to date.

Budget closed at 97% of plan. Headcount remained stable with one open SRE role that we expect to fill in Q2.

**Scorecard**

| Commitment | Target | Actual | Status |
|---|---|---|---|
| NOC Dashboard Launch | March 31 | March 28 | ✅ |
| P1 Incident Reduction | 25% ↓ | 31% ↓ | ✅ |
| Runbook Coverage | 80% | 78% | 🟡 |
| VoIP Phase 2 UAT Start | March 17 | Delayed to April 21 | 🔴 |
| Budget Utilization | 100% | 97% | ✅ |

**Q2 Look Ahead**
Primary focus: complete VoIP Phase 2 and begin planning for site decommissioning. Key risk is continued vendor dependency on hardware lead times.

**Anticipated Questions**
- *"Is the VoIP delay going to impact the Q2 customer commitment?"* → No — we built a 3-week buffer into the customer-facing date. We're tracking to the original external deadline.
- *"Why is runbook coverage still below target?"* → Two node types required vendor documentation we received late. Both are now in review and will be complete by April 15.

---

## Prompt 2 — One-Page Program Brief (for New Stakeholders)

```
You are a Technical Program Manager creating a one-page brief for a new executive stakeholder joining the program.

Program name: [name]
New stakeholder's role: [e.g., "New VP of Engineering taking over the portfolio"]
What they need to know fast: [top 3 things that matter most]
Program status: [current phase, health, timeline]
Team involved: [key roles and names]
Recent decisions made: [list 2–3 important decisions already locked]
Open decisions they'll need to weigh in on: [list]
Risks they should know about immediately: [list]

Please write a one-page brief that:
1. Gives them enough context to contribute in their first meeting
2. Doesn't assume prior knowledge
3. Clearly flags what needs their attention now vs. what can wait
4. Ends with a suggested first action for them to take
```

---

## Prompt 3 — Leadership Decision Memo

```
You are a Technical Program Manager writing a decision memo for leadership.

Decision needed: [describe the choice that needs to be made]
Background: [why this decision is coming up now]
Option A: [describe] — Pros: [list] — Cons: [list] — Cost/effort: [estimate]
Option B: [describe] — Pros: [list] — Cons: [list] — Cost/effort: [estimate]
Option C (if applicable): [describe]
Your recommendation: [which option and why]
Deadline for decision: [when does this need to be decided to avoid impact?]
Who is affected by this decision: [teams, customers, systems]

Write a decision memo that:
1. Opens with the recommended decision in the first sentence
2. Presents the options fairly before making the case for your recommendation
3. Is scannable — leadership should be able to read it in under 3 minutes
4. Ends with a clear call to action: "To proceed, please reply with your approval by [date]"
```

---

## Prompt 4 — Program Status Dashboard Narrative

```
You are a Technical Program Manager writing a recurring leadership dashboard update.

Program: [name]
Reporting period: [e.g., Week of April 7]
Overall status: [Green / Yellow / Red]

Workstream updates:
1. [Workstream name] — Status: [G/Y/R] — Update: [1–2 sentences]
2. [Workstream name] — Status: [G/Y/R] — Update: [1–2 sentences]
3. [Add more as needed]

Key metrics this week:
- [Metric 1]: [value] vs. [target]
- [Metric 2]: [value] vs. [target]

Escalations needed: [yes/no — describe if yes]
Decisions needed this week: [list or "none"]

Generate a dashboard narrative that:
1. Is under 200 words
2. Leads with overall health and one-line rationale
3. Uses consistent formatting week over week (so readers can scan fast)
4. Flags anything needing human action in bold
```

---

## Tips for Using These Prompts

- For QBRs (Prompt 1): Leadership remembers the story, not the data. Lead with outcomes and let the scorecard do the detail work.
- For Prompt 2: First impressions with new executives matter. This brief is also a great artifact for your portfolio.
- Decision memos (Prompt 3) are one of the highest-leverage TPgM skills. Executives who get clean, structured decisions make faster calls — and they remember who made it easy.
- Dashboard narratives (Prompt 4): Consistency beats perfection. Send the same format every week and stakeholders learn to trust it.
