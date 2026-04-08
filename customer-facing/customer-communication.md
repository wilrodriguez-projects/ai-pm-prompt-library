# 💬 Customer Communication Prompts

**Role:** Technical Program Manager / Customer-Facing Lead  
**Category:** Customer Communication  
**Use when:** Communicating outages, delays, feature updates, or any change that affects customers directly. Also useful for proactive outreach and relationship updates.

---

## Prompt 1 — Outage or Service Disruption Notice

```
You are a Technical Program Manager writing an outage communication for affected customers.

What happened: [describe the issue in plain terms]
Services affected: [list what's impacted]
Customer impact: [what can't they do right now?]
Start time: [when did it begin?]
Current status: [actively investigating / identified / fix in progress / resolved]
Estimated resolution time: [if known — if not, say "we'll update every 30 minutes"]
Root cause (if known): [brief, plain-language description]
Next update time: [when will you communicate again?]

Write a customer-facing outage notice that:
1. Opens with a direct statement of the issue — no corporate softening
2. Acknowledges customer impact empathetically
3. Gives a concrete next update time
4. Avoids technical jargon
5. Is appropriate for [choose: email / status page / SMS / Slack community]
```

---

### 📄 Example Output

**Prompt used:** Outage Notice — VoIP Service Degradation

---

**Subject: VoIP Service Degradation — We're On It**

We're aware that some customers are experiencing dropped calls and degraded call quality on our VoIP platform starting at approximately 2:14 PM ET today.

**What's affected:** Inbound and outbound call routing for customers in the Northeast region.

**What we're doing:** Our network operations team identified the issue at 2:22 PM and is actively working to restore full service. We've isolated the problem to a routing misconfiguration introduced during today's maintenance window and have a fix in testing now.

**What you can do in the meantime:** Calls can be temporarily redirected to mobile backup numbers if your team needs immediate coverage. Contact your account manager for assistance with that setup.

**Next update:** We will post another update by 4:00 PM ET or sooner if the issue is resolved.

We understand this is disrupting your operations and we take that seriously. We'll share a full incident summary within 24 hours of resolution.

— Wil Rodriguez, Network Operations Program

---

## Prompt 2 — Proactive Delay or Change Notification

```
You are a Technical Program Manager notifying customers of a delay or change to a committed timeline.

What was committed: [what the customer was expecting and when]
What changed: [what is now happening instead]
Reason for the change: [honest, simple explanation — don't over-explain]
New timeline: [updated delivery date or next milestone]
Impact on the customer: [what does this mean for them practically?]
What you're doing to prevent further slippage: [concrete steps]
Who to contact with questions: [name / email / Slack]

Write a notification that:
1. Leads with the change — don't bury the news
2. Is honest without being alarming
3. Shows the customer you have a plan
4. Offers a clear point of contact
5. Does not use passive voice or blame external factors without owning the response
```

---

## Prompt 3 — Feature or Change Announcement

```
You are a Technical Program Manager announcing a new feature, product update, or operational change to customers.

What's changing or launching: [name and brief description]
Effective date: [when does this take effect?]
Who is affected: [all customers / specific segment / specific accounts]
What's better for them: [key benefit — lead with value, not features]
What they need to do (if anything): [action required / no action required]
Where to get more information: [docs link, FAQ, support contact]
Tone: [e.g., "excited launch" / "routine update" / "required compliance change"]

Write a customer announcement that:
1. Opens with the customer benefit, not the technical change
2. Is appropriately short — customers don't read long emails
3. Has a clear subject line suggestion
4. Ends with one obvious next step or CTA
```

---

## Prompt 4 — Executive-Level Customer Update (Strategic Account)

```
You are a Technical Program Manager preparing an update for a strategic enterprise customer's leadership team.

Customer name: [company name — or use "the customer" if confidential]
Relationship context: [how long have they been a customer, what do they use, what matters to them]
What's been happening recently: [project progress, issues, wins]
What you want to accomplish with this update: [reassure / realign / escalate / celebrate progress]
Key metrics to share: [uptime, ticket resolution time, project milestones, etc.]
Open issues or concerns: [anything that might come up — address proactively]
Your ask or next step from them: [renewal conversation / feedback / decision on scope]

Write an executive update that:
1. Opens with a relationship acknowledgment, not a status dump
2. Leads with outcomes and value delivered
3. Addresses known concerns directly — don't wait for them to bring it up
4. Ends with a clear ask or proposed next conversation
5. Tone: warm, professional, confident — peer to peer, not vendor to client
```

---

## Tips for Using These Prompts

- Outage comms (Prompt 1): Speed matters more than perfection. A fast, honest update beats a polished one that takes an hour to draft.
- Delay notifications (Prompt 2): Customers handle bad news better when they hear it from you first and you come with a plan.
- Feature announcements (Prompt 3): Always answer "what's in it for me?" in the first sentence. Everything else is supporting detail.
- Prompt 4 is the highest-stakes communication in this file. Use it before QBRs, renewal conversations, or after a major incident with a key account.
