# 🎯 OKRs & Goals Prompts

**Role:** Technical Program Manager  
**Category:** Goal Setting & OKR Planning  
**Use when:** Writing quarterly OKRs, aligning team goals to company strategy, tracking key results, or presenting goal progress to leadership.

---

## Prompt 1 — Write Quarterly OKRs

```
You are a Technical Program Manager writing OKRs for the upcoming quarter.

Team or function: [e.g., "Platform Engineering" / "Customer Operations" / "Network Reliability"]
Quarter: [e.g., Q3 2025]
Company or org-level priority this quarter: [e.g., "Reduce customer churn" / "Scale infrastructure to support 2x users"]
What your team is responsible for: [brief description of scope]
Major initiatives planned this quarter: [list]
Last quarter's biggest gap or miss: [1–2 sentences]

Please generate:
1. 3 Objectives — each should be qualitative, inspirational, and outcome-focused (not a task list)
2. 3–4 Key Results per Objective — each should be measurable, time-bound, and binary (done or not done)
3. A confidence check: flag any KR that seems unrealistic or unmeasurable
4. One "stretch" KR per Objective — ambitious but not impossible
5. A one-paragraph OKR summary I can share with my manager for alignment before finalizing
```

---

### 📄 Example Output

**Prompt used:** Q3 OKRs — Network Reliability Team

---

**Objective 1: Make our network the most reliable in the region**
- KR1: Reduce P1 incidents by 40% vs. Q2 baseline (from 18 to ≤11)
- KR2: Achieve 99.95% uptime across all Tier 1 circuits by Sept 30
- KR3: Complete NOC runbook coverage for 100% of critical node types (currently 60%)
- ⭐ Stretch KR: Deploy automated alerting for top 5 failure patterns, reducing MTTR by 25%

**Objective 2: Accelerate how fast we respond when things go wrong**
- KR1: Reduce mean time to acknowledge (MTTA) from 18 min to under 8 min
- KR2: Conduct and document 3 tabletop incident exercises with cross-functional teams
- KR3: 100% of P1/P2 incidents have a completed postmortem within 5 business days
- ⭐ Stretch KR: Publish shared incident dashboard visible to CS and Engineering by Aug 15

**Confidence Check**
- KR on uptime (99.95%) is aggressive given current vendor SLA constraints — recommend flagging as dependency-based
- Runbook coverage KR is achievable but requires 2 dedicated engineer-days per week

**Summary for Manager**
This quarter our OKRs focus on two compounding outcomes: fewer incidents and faster recovery when they happen. The reliability target is ambitious but grounded in Q2 learnings. We've built in one vendor dependency flag and one stretch KR per objective to push the team without overcommitting. Ready to align before Q3 kickoff.

---

## Prompt 2 — OKR Check-In & Mid-Quarter Review

```
You are a Technical Program Manager running a mid-quarter OKR check-in.

Quarter: [e.g., Q3 2025]
Weeks into the quarter: [e.g., Week 6 of 13]

Current OKRs and progress:
Objective 1: [name]
  - KR1: [description] — Progress: [e.g., 60% / On Track / At Risk / Off Track]
  - KR2: [description] — Progress: [...]
  - KR3: [description] — Progress: [...]

Objective 2: [name]
  - KR1: [description] — Progress: [...]
  [continue...]

What's blocking progress on any At Risk or Off Track KRs: [describe]

Please generate:
1. A mid-quarter OKR scorecard with RAG status per KR
2. A forecast: based on current pace, which KRs will hit, which will miss
3. Recommended actions to recover any At Risk KRs (with owners)
4. A decision: which KRs should be deprioritized if trade-offs are needed
5. A mid-quarter update message suitable for sharing with leadership
```

---

## Prompt 3 — Align Team Goals to Company Strategy

```
You are a Technical Program Manager helping connect team-level work to company-level strategy.

Company strategic priorities this year: [list 2–4 top-level company goals]
Your team's planned work this quarter: [list key initiatives and projects]
Your team's function: [what does your team do and who do they serve?]

Please:
1. Map each team initiative to a company strategic priority (show the connection clearly)
2. Identify any team work that doesn't connect to company priorities (potential deprioritization candidates)
3. Identify any company priority that your team has NO work supporting (potential gap)
4. Write a "strategic alignment narrative" — 2–3 sentences I can use in leadership reviews to show how my team's work ladders up
5. Suggest one initiative my team could add or reprioritize to better serve the top company priority
```

---

## Prompt 4 — End-of-Quarter OKR Retrospective

```
You are a Technical Program Manager closing out a quarter's OKRs.

Quarter: [e.g., Q2 2025]

Final OKR scores:
Objective 1: [name] — Final score: [0.0–1.0 or %]
  - KR1: [description] — Result: [what actually happened]
  - KR2: [description] — Result: [...]

Objective 2: [name] — Final score: [...]
  [continue...]

What went well this quarter: [list]
What got in the way: [list]
Surprises (good or bad): [list]

Please generate:
1. A quarter closeout summary with honest scoring commentary
2. Root cause analysis for any KR scored below 0.7
3. Carry-forward recommendations: which KRs should roll into next quarter
4. Insights to feed into next quarter's OKR-writing process
5. A 3-minute verbal summary I could deliver in an all-hands or leadership review
```

---

## Tips for Using These Prompts

- Good OKRs are hard to write. Prompt 1 is best used with a manager or peer to pressure-test before finalizing.
- The "confidence check" in Prompt 1 is intentionally critical — don't skip it. It catches wishful thinking early.
- Mid-quarter check-ins (Prompt 2) are where OKRs actually drive behavior. Weekly is better than monthly.
- Prompt 3 is underused — but being able to articulate how your team's work connects to company strategy is a career accelerator.
