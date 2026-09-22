# Harvest questions worth answering

**Area:** Keyword research and clustering

**When.** Paste this when you want a list of real questions to answer, ranked by the demand you can already see.

## Prompt

```
Below are two inputs: my Search Console Queries export for the last 12 months (query, clicks, impressions, position) and a list of People Also Ask questions I collected for my main topic. If either is missing, ask me for it before doing anything.

Harvest questions. From the export, keep only queries that start with how, what, why, when, which, can, does, is, or should, and have at least 30 impressions. From the People Also Ask list, keep every question. Merge duplicates worded differently. Mark each question as answered (I rank in position 1 to 10), weak (position 11 to 30), or missing (no position, or only in the People Also Ask list).

Output a table, max 30 rows, sorted by impressions descending with People Also Ask only rows at the end, columns: question, source (GSC, PAA, both), impressions, position, status, suggested home (existing page URL or new page). If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the one question to answer this week and where, no alternatives.
```
