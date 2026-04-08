# 📈 Dashboard & Visualization Planning Prompts

**Role:** Data Analyst  
**Category:** Dashboard Design & Data Visualization  
**Use when:** Designing a new dashboard, choosing the right chart types, planning a KPI view, or presenting data visually for different audiences.

---

## Prompt 1 — Dashboard Design Blueprint

```
You are a data analyst designing a dashboard from scratch.

Dashboard name: [e.g., "Customer Health Dashboard"]
Primary audience: [e.g., Customer Success Managers / Sales leadership / Engineering team]
How often will it be used: [e.g., daily / weekly / ad hoc]
Key questions this dashboard must answer:
1. [Question 1]
2. [Question 2]
3. [Question 3]

Data available: [list the tables or data sources]
Tool being used: [e.g., Tableau / Looker / Power BI / Metabase / Google Data Studio]
Time filters needed: [e.g., last 7/30/90 days, date range picker, rolling vs. fixed]

Please generate:
1. A recommended dashboard layout (sections, panels, and their purpose)
2. A list of visualizations for each section with chart type and why that type fits
3. KPIs to feature at the top (summary numbers with context)
4. Drill-down suggestions: what should users be able to click into for more detail?
5. Design principles to follow for this audience (what to simplify, what to highlight)
```

---

## Prompt 2 — KPI Selection & Definition

```
You are a data analyst helping define the right KPIs for a team or product area.

Team or function: [e.g., "Customer Support" / "Growth team" / "Payments product"]
Business objective: [e.g., "Improve customer retention" / "Increase conversion rate"]
What decisions will these KPIs drive: [describe how leaders will use them]
Data available to calculate metrics: [list tables and key columns]
Cadence for review: [weekly / monthly / quarterly]

Please:
1. Recommend 4–6 KPIs that best represent health and performance for this area
2. For each KPI, provide:
   - Name
   - Definition (how it's calculated — be precise)
   - Why it matters
   - Target or benchmark (if inferable)
   - Leading vs. lagging indicator classification
   - SQL or formula sketch to calculate it
3. Flag any vanity metrics to avoid for this use case
4. Suggest one "north star" metric that best summarizes overall success
```

---

## Prompt 3 — Choose the Right Chart Type

```
You are a data analyst advising on data visualization best practices.

What I'm trying to show: [e.g., "How revenue changed week over week for 3 product lines over the last 6 months"]
Data structure:
- X-axis candidate: [e.g., week / date]
- Y-axis candidate: [e.g., revenue in $]
- Breakdown / grouping: [e.g., by product line]
- Number of data points: [e.g., ~26 weeks × 3 lines = 78 points]
Audience: [technical / non-technical / exec]
Tool: [e.g., Tableau / Python matplotlib / Google Sheets / Looker]

Please:
1. Recommend the best chart type for this data and explain why
2. List 2 alternative chart types and when you'd choose them instead
3. Describe specific design choices: colors, labels, gridlines, annotations
4. Warn me about common mistakes for this chart type (e.g., dual-axis abuse, truncated Y-axis)
5. Write a one-sentence chart title that is insight-driven, not just descriptive
   (e.g., "Revenue grew fastest in Product Line B for 4 straight weeks" vs. "Revenue by Product Line")
```

---

## Prompt 4 — Dashboard Audit & Improvement Plan

```
You are a data analyst reviewing an existing dashboard that isn't being used effectively.

Dashboard name: [name]
Current audience: [who it's for]
Problem: [e.g., "Team doesn't use it regularly" / "Takes too long to load" / "Stakeholders say it's confusing"]
Current charts / panels: [describe or list what's currently on the dashboard]
Data freshness: [how often does data refresh?]
Tool: [Tableau / Looker / Power BI / etc.]

Please generate:
1. Likely reasons why this dashboard isn't being used effectively
2. Specific improvements for each panel (remove, replace, reframe, or simplify)
3. Layout recommendations to reduce cognitive load
4. Performance improvements if load time is an issue
5. A stakeholder interview guide (3–5 questions) to ask the audience before redesigning
```

---

## Tips for Using These Prompts

- Prompt 1: Before building anything, get the audience to answer "what decision will this help you make?" — that answer drives everything else.
- Prompt 2: Fewer, well-defined KPIs beat large scoreboards. Aim for 5–6 max per dashboard.
- Prompt 3: The best chart title answers the question "what should I take away from this?" not "what is plotted here?"
- Prompt 4: Low dashboard adoption is almost always a design problem or a trust problem (stale data). Use this prompt to diagnose before rebuilding.
