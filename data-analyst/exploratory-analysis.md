# 🔍 Exploratory Analysis Prompts

**Role:** Data Analyst  
**Category:** Data Exploration & Profiling  
**Use when:** Working with a new dataset, investigating a business question, profiling data quality, or looking for patterns before a deeper analysis.

---

## Prompt 1 — Dataset Profiling & First Look

```
You are a data analyst profiling a dataset for the first time before doing deeper analysis.

Dataset name or source: [e.g., "customer_orders table" / "exported CSV from Salesforce"]
Number of rows (approx): [e.g., ~500K rows]
Number of columns: [e.g., 22 columns]
Column names and types:
[paste column names and their data types here, or describe them]

Business context: [What is this data used for? What does one row represent?]

Please generate:
1. A data profiling checklist — what to check before trusting this data
2. Key questions to investigate early (nulls, duplicates, outliers, unexpected distributions)
3. A list of SQL queries or Python code I should run to profile each column type
4. Red flags to watch for that would indicate data quality problems
5. A first-look summary template I can fill in after running the checks
```

---

## Prompt 2 — Exploratory Data Analysis (EDA) Plan

```
You are a data analyst planning an exploratory data analysis for a new business question.

Business question: [e.g., "Why are customers in the Western region churning at a higher rate?"]
Dataset(s) available: [list tables or files]
Key columns relevant to the question: [list]
Time period to analyze: [e.g., last 6 months]
What we already know or suspect: [any hypotheses or prior context]

Please create an EDA plan that includes:
1. Analysis objectives (what we're trying to learn)
2. Step-by-step exploration sequence (what to look at first, second, third)
3. Suggested breakdowns and segmentations (by time, region, product, customer type, etc.)
4. Metrics to calculate at each step
5. What "interesting" looks like — signals that would be worth digging into further
6. What "nothing to see here" looks like — conditions where we'd move on
```

---

## Prompt 3 — Outlier & Anomaly Investigation

```
You are a data analyst investigating unusual patterns or outliers in a dataset.

Dataset / metric in question: [e.g., "daily transaction volume", "user session length"]
What looks unusual: [describe the anomaly — spike, drop, impossible values, etc.]
Time period affected: [e.g., "March 15–22, 2025"]
Affected segment (if known): [e.g., "enterprise accounts" / "mobile platform only"]
Data source: [where this data comes from — warehouse table, API feed, etc.]

Please:
1. Generate a list of likely explanations for this anomaly (ranked by probability)
2. For each explanation, suggest a specific SQL query or data check to test it
3. Identify whether this is likely a data quality issue vs. a real business signal
4. Describe how to document and communicate this finding before conclusions are drawn
5. Suggest monitoring logic to detect similar anomalies in the future
```

---

## Prompt 4 — Cohort Analysis Setup

```
You are a data analyst setting up a cohort analysis to understand customer behavior over time.

Business question: [e.g., "Do customers who onboard in Q4 retain better than Q1 cohorts?"]
Cohort definition: [e.g., "users grouped by the month they first made a purchase"]
Metric to track: [e.g., "retention rate", "repeat purchase rate", "monthly revenue per user"]
Time horizon: [e.g., "track each cohort for 12 months post-acquisition"]

Relevant tables:
- [table_name] — key columns: [list]
- [table_name] — key columns: [list]

Please:
1. Explain the cohort analysis approach in plain English (suitable for sharing with a non-technical stakeholder)
2. Write the SQL to build the cohort table (with clear CTEs and comments)
3. Describe what output the query produces and how to read it
4. Suggest how to visualize the results (chart type, axes, what to highlight)
5. Flag any edge cases in the data that could skew the cohort results
```

---

## Tips for Using These Prompts

- Always run Prompt 1 before any other analysis — bad data leads to confident wrong answers.
- Prompt 2 is your analysis blueprint. Share it with your manager before diving deep to confirm you're solving the right problem.
- Prompt 3 is your "fire drill" prompt — use it when something looks off and you need to triage fast.
- Cohort analyses (Prompt 4) are one of the highest-signal tools in a DA toolkit. They show customer behavior trends that averages completely hide.
