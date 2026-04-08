# 🗃️ Portfolio Planning Prompts

**Role:** Technical Program Manager  
**Category:** Portfolio & Program Planning  
**Use when:** Managing multiple projects simultaneously, building a program roadmap, prioritizing across workstreams, or reporting portfolio health upward.

---

## Prompt 1 — Program Portfolio Overview

```
You are a Technical Program Manager responsible for a portfolio of projects.

Program/portfolio name: [e.g., "Network Modernization Program"]
Number of active projects: [e.g., 5]
Total team size across projects: [e.g., ~30 people across 4 teams]
Timeframe: [e.g., Q2–Q4 2025]

Projects in the portfolio:
1. [Project name] — Goal: [one line] — Status: [Green/Yellow/Red] — Phase: [e.g., planning/execution/closeout]
2. [Project name] — Goal: [one line] — Status: [Green/Yellow/Red] — Phase: [...]
3. [Add more as needed]

Shared dependencies or constraints: [e.g., shared QA team, single infrastructure environment, budget cap]

Please generate:
1. A portfolio health summary (suitable for a leadership slide)
2. A dependency map narrative — which projects are blocking or dependent on each other
3. Top 3 cross-program risks
4. A recommended prioritization order with rationale
5. A 30-day focus recommendation: where should program leadership spend their attention first?
```

---

### 📄 Example Output

**Prompt used:** Portfolio Overview — Network Modernization Program (3 projects)

---

**Portfolio Health Summary**

The Network Modernization Program is tracking at **Yellow** overall. Two of three active workstreams are on schedule; the Core Infrastructure Upgrade has slipped to Yellow due to a vendor delivery delay impacting the shared lab environment.

**Dependency Map**
- The VoIP Migration (Phase 2) cannot begin UAT until Core Infrastructure Upgrade completes lab provisioning — currently delayed by 2 weeks.
- The NOC Dashboard project has no hard dependencies but shares QA resources with VoIP Migration, creating a soft capacity risk in weeks 3–4.

**Top 3 Cross-Program Risks**
1. Vendor delay on lab environment — impacts VoIP UAT start date (High)
2. QA team overallocation in weeks 3–4 — may require staggered test windows (Medium)
3. No fallback vendor identified for hardware procurement (Medium)

**Prioritization Order**
1. Core Infrastructure Upgrade — unblocks downstream work
2. VoIP Migration Phase 2 — highest customer visibility
3. NOC Dashboard — lowest dependency footprint, can absorb a 1-week slip if needed

**30-Day Focus Recommendation:** Resolve vendor delay and formally document QA schedule across all three projects before the next planning cycle.

---

## Prompt 2 — Program Roadmap Builder

```
You are a Technical Program Manager building a multi-quarter program roadmap.

Program name: [e.g., "Customer Platform Transformation"]
Program goal: [What does success look like at the end of this program?]
Duration: [e.g., 12 months / 3 quarters]
Key workstreams: [list each major track of work]
Known milestones: [list any fixed dates — launches, audits, contracts, etc.]
Resource constraints: [budget, headcount, technology limits]
Stakeholders who will see this roadmap: [e.g., CTO, VP Product, Finance]

Please generate:
1. A quarter-by-quarter roadmap narrative (Q1 / Q2 / Q3 themes and goals)
2. Key milestones per quarter with owners
3. Dependencies between workstreams shown as a sequencing narrative
4. A "what could go wrong" summary per quarter
5. Success criteria for the end of the program
```

---

## Prompt 3 — Resource Allocation Across Projects

```
You are a Technical Program Manager managing shared resources across multiple projects.

Total available capacity: [e.g., 8 engineers, 2 QA, 1 designer — all full-time]
Projects competing for resources:
1. [Project A] — needs: [X engineers, Y QA] — priority: [High/Med/Low] — deadline: [date]
2. [Project B] — needs: [X engineers, Y QA] — priority: [High/Med/Low] — deadline: [date]
3. [Add more]

Constraints:
- [e.g., "Engineer 3 is on PTO weeks 2–3"]
- [e.g., "QA cannot run two projects simultaneously in the same environment"]

Please generate:
1. A recommended resource allocation plan by week or sprint
2. Conflicts identified — where demand exceeds supply
3. Trade-off options for over-allocated periods
4. A capacity summary I can present to leadership to justify a hire or delay
```

---

## Prompt 4 — Program Closeout & Lessons Learned

```
You are a Technical Program Manager closing out a completed program.

Program name: [name]
Duration: [start date → end date]
Original goals: [what the program set out to achieve]
Actual outcomes: [what was delivered — be honest about gaps]
Budget: [planned vs. actual]
Timeline: [planned vs. actual]
Team involved: [list roles/teams]
Top 3 things that went well: [list]
Top 3 things that didn't go as planned: [list]

Please generate:
1. A program closeout summary (shareable with leadership and stakeholders)
2. Lessons learned document (blameless, structured for future program teams)
3. Metrics comparison: planned vs. actual for scope, schedule, and budget
4. Recommendations for the next program of similar type
5. Recognition talking points for the team (genuine, specific — not generic)
```

---

## Tips for Using These Prompts

- Prompt 1 works best run weekly — keep a live version of your project status bullets and refresh it each Monday.
- Prompt 2: Build the roadmap before stakeholders ask for it. Proactive roadmap sharing is a TPgM superpower.
- Prompt 3: Resource conflicts are easier to solve on paper than mid-sprint. Use this monthly.
- Prompt 4: Closeout docs are often skipped — but they're gold for your portfolio and for the next person who runs a similar program.
