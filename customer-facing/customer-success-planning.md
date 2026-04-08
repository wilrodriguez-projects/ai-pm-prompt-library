# 🌱 Customer Success Planning Prompts

**Role:** Technical Program Manager / Customer-Facing Lead  
**Category:** Customer Success & Retention Planning  
**Use when:** Building success plans for key accounts, preparing for QBRs with customers, tracking customer health, or proactively managing at-risk accounts.

---

## Prompt 1 — Customer Success Plan

```
You are a Technical Program Manager building a success plan for a strategic customer account.

Customer name: [company name]
Account size / ARR: [e.g., $150K ARR]
Contract term: [e.g., 2-year contract, renews January 2026]
Products / services they use: [list]
Customer's stated business goals: [what are they trying to achieve with your product/service?]
Current adoption level: [e.g., "using 60% of available features", "3 of 5 locations onboarded"]
Known risks: [e.g., "champion leaving the company", "low executive sponsorship", "billing dispute in Q3"]
Upcoming milestones: [renewal date, planned expansions, new use cases]

Please generate:
1. A 90-day success plan with weekly focus areas
2. Adoption gaps to address and recommended actions
3. Health score assessment: Green / Yellow / Red with rationale
4. Key relationships to build or strengthen
5. 3 ways to demonstrate value before the renewal conversation
```

---

## Prompt 2 — Customer QBR Prep (Your Side)

```
You are a Technical Program Manager preparing your team for a Quarterly Business Review with a customer.

Customer name: [name]
QBR date: [date]
Attendees — customer side: [names and roles]
Attendees — your side: [names and roles]
Quarter being reviewed: [e.g., Q1 2025]

What went well this quarter: [list with data if possible]
What didn't go well (be honest): [list]
Metrics to present: [SLA performance, uptime, ticket volume, adoption metrics, etc.]
Customer's known concerns or priorities: [what do they care most about?]
What you want to walk out of the QBR with: [agreement on something / expansion conversation / feedback]

Please generate:
1. A QBR agenda (60-minute format)
2. A "value delivered" narrative — frame the quarter from the customer's perspective
3. How to address the negative items proactively (before they bring it up)
4. A slide-by-slide outline with suggested talking points
5. Questions to ask the customer to learn what they need next
```

---

### 📄 Example Output

**Prompt used:** Customer QBR Prep — Regional Healthcare Provider, Q1 2025

---

**QBR Agenda (60 min)**
- 0–5 min: Welcome, introductions, agenda overview
- 5–15 min: Q1 Performance Review — SLA, uptime, support metrics
- 15–25 min: Value Delivered — key milestones and business outcomes
- 25–35 min: Open Items & Issue Review — address the March outage directly
- 35–45 min: Your Roadmap — what's coming in Q2 that matters to them
- 45–55 min: Their Goals — what does success look like for Q2?
- 55–60 min: Next steps, action items, close

**Value Delivered Narrative**
This quarter your team maintained 99.91% uptime across all call routing — your highest quarter since onboarding. We resolved 94% of tickets within SLA, up from 87% in Q4. The March 7 routing issue was the exception, not the rule, and we've put two specific controls in place to prevent a recurrence. Your NOC team now has direct escalation access to our senior engineering queue, which reduces response time by an estimated 40%.

**Addressing the March Outage (Proactively)**
Don't wait for them to bring it up. Open slide 3 with: *"Before we get into the numbers, we want to address the March 7 incident directly. Here's what happened, what we found, and what we changed."* Customers respect teams that own their misses. Trying to minimize it damages trust more than the outage itself.

**Questions to Ask**
1. What does a successful Q2 look like for your operations team?
2. Are there use cases you're not currently solving with our platform that you wish you could?
3. Who else in your organization should be in these conversations?

---

## Prompt 3 — At-Risk Account Recovery Plan

```
You are a Technical Program Manager building a recovery plan for a customer account at risk of churning.

Customer name: [name]
Risk signals: [list what's happening — low usage, support complaints, exec disengagement, competitor evaluation, etc.]
When renewal is: [date]
Current relationship health: [Red / very Yellow]
What the customer has said (if anything): [direct feedback or complaints]
What we believe is really going on: [your honest internal read]
What we've tried so far: [list previous outreach or fixes]
Internal champion (if any): [who inside the customer still believes in you?]

Please generate:
1. A 60-day account recovery plan with weekly milestones
2. Root cause hypothesis: what is actually driving the risk?
3. The "win-back" moment: what single action would most shift the customer's perception?
4. An outreach message to reopen the relationship (not a sales pitch — a genuine check-in)
5. Escalation trigger: at what point do we involve executive leadership on our side?
```

---

## Prompt 4 — Customer Onboarding Plan

```
You are a Technical Program Manager building an onboarding plan for a new customer.

Customer name: [name]
Product / service they're onboarding to: [name and brief description]
Contract start date: [date]
Customer's team involved in onboarding: [roles and names if known]
Your team involved: [roles]
Customer's primary goal for onboarding: [what does "done" look like for them?]
Known complexity or risk: [e.g., "they're migrating from a legacy system", "3 locations with different configs"]
Timeline committed: [when should they be fully live?]

Please generate:
1. A phased onboarding plan (Week 1 / Weeks 2–3 / Weeks 4–6 / Go-Live)
2. Success criteria for each phase
3. Customer responsibilities vs. your team's responsibilities (RACI-style)
4. Top 3 onboarding risks and how to mitigate them
5. A "Day 1" welcome message to send the customer when they sign
```

---

## Tips for Using These Prompts

- Success plans (Prompt 1) are living documents — review them monthly, not just at renewal time.
- QBR prep (Prompt 2): The best QBRs feel like a conversation between partners, not a vendor presentation. Lead with their goals, not your metrics.
- At-risk recovery (Prompt 3): Start the recovery plan the moment you see the signals — not 30 days before renewal.
- Prompt 4: Onboarding sets the tone for the entire customer relationship. A structured plan in week 1 prevents half the escalations in month 6.
