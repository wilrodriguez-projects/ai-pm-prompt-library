# 🛠️ Support & Planning Prompts

**Role:** Technical Program Manager / Customer-Facing Lead  
**Category:** Support Operations & Customer Planning  
**Use when:** Structuring support workflows, writing knowledge base articles, planning capacity for support teams, or translating technical fixes into customer-friendly documentation.

---

## Prompt 1 — Support Ticket Response (Technical Issue)

```
You are a Technical Program Manager or senior support lead responding to a customer technical support ticket.

Customer name: [name or "customer"]
Issue reported: [what the customer said, as close to verbatim as possible]
Ticket severity: [P1 / P2 / P3 / P4]
What we know so far: [investigation findings]
Resolution status: [investigating / identified / fix in progress / resolved]
Fix or workaround available: [describe, or "not yet"]

Write a support response that:
1. Acknowledges the customer's experience in the first sentence
2. Gives an honest status update — no corporate fluff
3. Provides a workaround if one exists
4. Sets a clear expectation for next update or resolution timeline
5. Is written in plain English — no jargon the customer can't act on
6. Tone: [choose: empathetic and urgent / professional and calm / brief and direct]
```

---

### 📄 Example Output

**Prompt used:** Support Response — P2 Call Routing Failure

---

Hi [Customer Name],

Thank you for reaching out — I can see this is affecting your inbound call flow and I want to make sure we resolve it quickly.

**What we've found:** Our team identified a routing table misconfiguration that's causing a subset of inbound calls to fail on transfer to your hunt group. This appears to be isolated to calls coming through the 800 number provisioned in March.

**What you can do right now:** As a temporary workaround, inbound calls can be directed to your direct DID numbers while we apply the fix. I can assist with redirecting that in the next 30 minutes if your team needs it.

**What we're doing:** The fix is being staged in our test environment now. We expect to deploy to production by 5:00 PM ET today. I'll confirm once it's in.

I'll update you again at 3:00 PM ET with a progress check. If anything changes before then, I'll reach out immediately.

— [Your name], Technical Support

---

## Prompt 2 — Knowledge Base Article (From Resolved Ticket)

```
You are a Technical Program Manager turning a resolved support ticket into a knowledge base article.

Issue title: [short description of the problem]
Affected product/system: [name]
Symptoms the customer experienced: [what they saw or reported]
Root cause: [what actually caused it — plain English]
Resolution steps: [exact steps taken to fix it]
Workaround (if applicable): [temporary fix while resolution is applied]
Affected versions or configurations: [e.g., "firmware v3.2.1", "accounts with SSO enabled"]
Prevention: [how to avoid this in the future]

Write a knowledge base article that:
1. Uses a clear, searchable title (starts with the symptom, not the cause)
2. Has a brief "What you'll see" section so customers can self-identify the issue
3. Provides step-by-step resolution instructions a non-technical user can follow
4. Includes a "When to contact support" note for cases where self-service isn't enough
5. Is formatted for easy scanning — short paragraphs, numbered steps
```

---

## Prompt 3 — Support Capacity & Coverage Planning

```
You are a Technical Program Manager planning support capacity for an upcoming period.

Team size: [number of support agents / engineers]
Coverage hours needed: [e.g., 8 AM–8 PM ET / 24x7 / follow-the-sun]
Expected ticket volume: [e.g., ~40 tickets/day based on last quarter]
Ticket mix: [e.g., 20% P1/P2, 50% P3, 30% P4]
Upcoming events affecting volume: [product launches, maintenance windows, holidays, migrations]
Current SLA targets: [P1: 1hr response / P2: 4hr / P3: 24hr]
Known gaps or risks: [e.g., "two agents on PTO weeks 3–4", "new product launching week 2"]

Please generate:
1. A weekly coverage plan with shift assignments
2. Volume forecast by week for the planning period
3. SLA risk assessment: which weeks are at risk of missing targets?
4. Overflow plan: what happens when volume spikes beyond capacity?
5. Staffing recommendation: do we need additional coverage for any period?
```

---

## Prompt 4 — Customer-Facing Maintenance Window Notice

```
You are a Technical Program Manager writing a planned maintenance notification for customers.

What's being maintained: [system, service, or infrastructure component]
Why it's needed: [brief explanation — upgrade, security patch, performance improvement]
Scheduled date and time: [include timezone]
Expected duration: [e.g., "approximately 2 hours"]
Customer impact during maintenance: [what will be unavailable or degraded?]
What customers should do: [any action required before/during/after]
Emergency contact during window: [who to call if something goes wrong]
Early completion plan: [will you notify if done early?]

Write a maintenance notice that:
1. States the date, time, and duration in the first two sentences
2. Clearly explains what customers will and won't be able to do
3. Is sent at least 72 hours in advance (note this in the communication)
4. Offers a contact for customers with concerns
5. Includes a "what to expect after maintenance" section
```

---

## Tips for Using These Prompts

- Ticket responses (Prompt 1): Write to the person, not the ticket. A response that acknowledges the customer's situation earns more goodwill than a technically perfect one that feels robotic.
- KB articles (Prompt 2): The best KB articles are written immediately after resolution, while the details are fresh. Schedule 15 minutes post-close to draft it.
- Capacity planning (Prompt 3): Run this 4–6 weeks ahead of any major product launch or seasonal spike — not the week before.
- Maintenance notices (Prompt 4): 72 hours minimum is the rule. Customers who feel informed are dramatically more tolerant of downtime than those who are surprised by it.
