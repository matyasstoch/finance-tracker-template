# Subscription Analysis

Source: `bank-statements/example-statement.csv` (6-month sample). Replace this table by asking your agent to parse your bank CSV.

Note: if the newest month is partial (for example, exported on the 15th), ignore charges that normally land later in the month.

## Monthly spend by category (USD)

```text
merchant              |Aug  |Sep  |Oct  |Nov  |Dec  |Jan* | run-rate
-- AI tools -----------------------------------------------------------
AI coding plan        | 100 | 100 | 100 | 100 | 100 | 100 | $100
AI APIs (usage)       |  85 | 120 | 165 | 210 | 240 | 140*| ~$240 (growing)
-- Hosting and dev ----------------------------------------------------
Supabase              |  25 |  25 |  25 |  25 |  38 |  25 | ~$30
Vercel                |  20 |  20 |  20 |  20 |  20 |  20 | $20
GitHub                |  25 |  25 |  25 |  25 |  25 |  25 | $25
-- Productivity / SaaS ------------------------------------------------
Google Workspace      |  15 |  15 |  15 |  15 |  15 |  15 | $15
Old analytics tool    |  35 |  35 |  35 |  35 |  35 |  35 | $35 -> CANCEL
Duplicate note app    |  20 |  20 |  20 |  20 |  20 |  20 | $20 -> CANCEL
```

## Takeaways

1. Usage-based AI APIs nearly tripled from August to December. Review prompts and set a hard monthly cap.
2. Cancelling the 2 unused SaaS tools saves $55/month ($660/year).
