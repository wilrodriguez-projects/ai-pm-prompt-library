# 🗃️ SQL Query Writing Prompts

**Role:** Data Analyst  
**Category:** SQL Query Generation & Optimization  
**Use when:** Writing queries from scratch, debugging slow queries, translating business questions into SQL, or reviewing someone else's code.

---

## Prompt 1 — Translate a Business Question into SQL

```
You are a data analyst. I have a business question I need to answer using SQL.

Database type: [e.g., PostgreSQL / BigQuery / Snowflake / MySQL / SQL Server]
Business question: [e.g., "What are the top 10 customers by revenue in the last 90 days?"]

Relevant tables and columns:
- Table: [table_name] — Columns: [col1, col2, col3, ...]
- Table: [table_name] — Columns: [col1, col2, col3, ...]

Any known filters or conditions: [e.g., "only active accounts", "exclude test users", "US region only"]

Please:
1. Write a clean, well-commented SQL query to answer the question
2. Explain what each major section of the query does (in plain English)
3. Flag any assumptions you made about the data
4. Suggest one alternative approach if there's a different way to answer this question
```

---

## Prompt 2 — Optimize a Slow Query

```
You are a senior data analyst reviewing a SQL query that's running too slowly.

Database type: [e.g., BigQuery / Snowflake / PostgreSQL]
Current query:
[paste your SQL here]

Table sizes (if known):
- [table_name]: ~[row count or size, e.g., "50M rows"]
- [table_name]: ~[row count or size]

Indexes available (if known): [list or "unknown"]
Current runtime: [e.g., "~45 seconds"]
Target runtime: [e.g., "under 5 seconds"]

Please:
1. Identify performance bottlenecks in the current query
2. Rewrite the query with optimizations applied
3. Explain each optimization and why it helps
4. Suggest any schema-level changes (indexes, partitioning) that would improve performance further
```

---

## Prompt 3 — Build a Reusable Reporting Query (CTE-Based)

```
You are a data analyst building a clean, reusable SQL query for a recurring report.

Database type: [e.g., Snowflake / BigQuery]
Report name: [e.g., "Weekly Active User Summary"]
Report goal: [What decision or metric does this report support?]
Grain of the report: [e.g., "one row per user per week" / "one row per day per product"]

Metrics needed:
- [Metric 1: name and definition, e.g., "Weekly Active Users = users with at least 1 session in the week"]
- [Metric 2: name and definition]
- [Metric 3: ...]

Filters: [e.g., "last 12 weeks", "active accounts only"]

Relevant tables: [list tables and key columns]

Please write a modular SQL query using CTEs (Common Table Expressions) that:
1. Is readable and self-documenting (with comments)
2. Is easy for another analyst to modify
3. Handles edge cases like nulls and division by zero
4. Includes a sample output description (column names and what each represents)
```

---

## Prompt 4 — Explain or Review Someone Else's SQL

```
You are a data analyst reviewing a SQL query written by someone else.

SQL to review:
[paste SQL here]

Context:
- What is this query supposed to do? [describe the intent]
- Database type: [e.g., PostgreSQL / BigQuery]
- Are there any known issues or surprising results? [yes/no — describe if yes]

Please:
1. Explain what this query actually does, step by step, in plain English
2. Identify any bugs, logic errors, or unexpected behaviors
3. Flag any style or readability issues
4. Suggest improvements to make it cleaner, safer, or more performant
5. Rewrite the corrected version if changes are needed
```

---

## Tips for Using These Prompts

- Always specify your database type — SQL syntax varies significantly between Snowflake, BigQuery, PostgreSQL, etc.
- For Prompt 1: The more specific your business question, the better the query. "Show me revenue" is weaker than "Show me total net revenue by account tier for the last 30 days."
- For Prompt 3: CTE-based queries are easier to maintain and more interview-friendly. Make this your default style.
- For Prompt 4: Great for onboarding onto a new team — use it to decode legacy queries fast.
