# 🚨 Escalation Management Prompts

**Role:** Technical Program Manager / Customer-Facing Lead  
**Category:** Customer Escalation Handling  
**Use when:** A customer is unhappy, a service issue has grown into a relationship risk, an SLA has been breached, or a situation requires executive involvement on either side.

---

## Prompt 1 — Escalation Triage & Response Plan

```
You are a Technical Program Manager triaging a customer escalation.

Customer name: [company or "strategic account"]
Escalation trigger: [what caused the escalation — outage, missed deadline, billing issue, product failure, etc.]
How the escalation surfaced: [customer email / executive call / account manager flag / social media]
Customer's stated concern: [what they said, as close to verbatim as possible]
Customer's actual concern (if different): [what you believe is really driving the frustration]
Business risk: [is this account at risk of churn / reducing spend / going to press?]
What's already been done: [any previous responses or attempts to resolve]
Internal owner: [who is leading resolution?]

Please generate:
1. An escalation severity rating (Critical / High / Medium) with rationale
2. A 24-hour response plan: who does what, in what order
3. An initial customer acknowledgment message (send within 1 hour)
4. A root cause investigation checklist
5. A stakeholder alert for internal leadership (brief, factual, no blame)
```

---

### 📄 Example Output

**Prompt used:** Escalation Triage — Enterprise Customer VoIP Outage Complaint

---

**Severity: High**
Rationale: Customer is a $240K ARR account, 3 years with us, experiencing their second VoIP disruption in 90 days. Their VP of Operations sent an email directly to our CTO this morning. No churn language yet, but the tone indicates trust erosion.

**24-Hour Response Plan**
- 0–1 hr: Send acknowledgment email to customer VP + CC account manager
- 0–2 hr: Pull incident timeline from NOC logs and identify if this is same root cause as prior event
- 2–4 hr: Internal call between Account Manager, TAM, and NOC lead to align on facts before customer call
- 4–6 hr: Schedule executive call with customer for tomorrow AM — do not leave this unscheduled
- EOD: Share internal incident summary with Customer Success leadership

**Customer Acknowledgment Message**
*[Name], thank you for reaching out directly. I've seen your note and want you to know this is my personal priority today. I'm pulling together our technical team to get a complete picture of what happened and what we're doing differently. I'll have a response for you by [time] today, and I'd like to schedule a call for tomorrow morning with our team to walk through it together. Does 10 AM work for you?*

**Internal Leadership Alert**
FYI: [Customer Name] escalated to the CTO following a VoIP disruption yesterday. This is their second incident in 90 days. AM and TAM are engaged. Root cause review in progress. No churn risk stated but relationship is strained. Will update by EOD.

---

## Prompt 2 — Customer Escalation Call Prep

```
You are a Technical Program Manager preparing for a customer escalation call.

Customer name: [name]
Who will be on the call — customer side: [names and roles]
Who will be on the call — your side: [names and roles]
What the customer is upset about: [specific issues they've raised]
What you know so far about root cause: [your findings to date]
What you've already done to address it: [actions taken]
What you cannot yet confirm or commit to: [open items]
Your goal for this call: [de-escalate / rebuild trust / get agreement on resolution plan / all three]

Please generate:
1. A call agenda (30–45 min)
2. An opening statement that acknowledges impact without over-apologizing
3. Talking points for each issue the customer raised
4. Answers to the 3 most likely tough questions they'll ask
5. A proposed close: what you want to walk away with agreed
6. What NOT to say — phrases or commitments to avoid
```

---

## Prompt 3 — Post-Escalation Resolution Summary

```
You are a Technical Program Manager writing a post-escalation summary for a customer.

Customer name: [name]
Original issue: [what the escalation was about]
What was found: [root cause, plain language]
What was done to fix it: [concrete steps taken]
Timeline of resolution: [when did each step happen]
What's being done to prevent recurrence: [specific, not vague]
Any compensation or goodwill gesture offered: [SLA credits, dedicated support, etc.]
Current relationship status: [resolved / cautiously positive / still at risk]

Write a post-escalation summary letter/email that:
1. Opens by acknowledging what the customer experienced
2. Explains what happened clearly without over-technicalizing
3. Shows a concrete prevention plan (not "we'll do better")
4. Closes warmly — reaffirm the relationship
5. Is written to the customer's decision-maker, not their technical contact
```

---

## Prompt 4 — Internal Post-Escalation Retrospective

```
You are a Technical Program Manager leading an internal retrospective after a customer escalation is resolved.

Customer impacted: [name or "Account A" if confidential]
Escalation summary: [what happened and how it was resolved]
Timeline: [key dates from trigger to resolution]
Teams involved: [list roles/teams]
How we found out about the issue: [customer reported / internal monitoring / account manager]
How quickly we responded: [first response time, time to resolution]
What we did well: [honest assessment]
What we should have done differently: [honest assessment]

Please generate:
1. A blameless retrospective document (structured for internal use)
2. Process gaps identified — where did our response system fail?
3. Early warning signals we missed — what should have flagged this sooner?
4. 3 specific action items with owners and due dates to prevent recurrence
5. A customer health score recommendation: should this account get elevated monitoring going forward?
```

---

## Tips for Using These Prompts

- Speed is the #1 thing customers remember in an escalation. Use Prompt 1 to generate your acknowledgment message in under 10 minutes.
- Never go into an escalation call without using Prompt 2 — walking in unprepared makes a bad situation worse.
- Prompt 3 is a relationship repair tool. A well-written post-escalation summary has saved more than a few accounts on the verge of churning.
- Internal retros (Prompt 4) only work if they're blameless. If people fear consequence, they'll hide information — and the next escalation will be worse.
