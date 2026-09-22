# Diff index coverage week over week

**Area:** Technical SEO and site audits

**When.** Paste this with two weekly exports of the indexing report when the indexed count moved and you want to know which URLs and why.

## Prompt

```
Below are two exports of the Search Console Pages indexing report (URL and its status or reason), one from last week and one from this week. If I pasted only one, ask me for the other before doing anything.

Diff them. Find: URLs that moved from indexed to not indexed, with the new reason; URLs that moved from not indexed to indexed; URLs new this week; URLs that disappeared from the report. Group by reason (crawled currently not indexed, discovered currently not indexed, noindex, redirect, soft 404, duplicate with Google chosen canonical, not found). Ignore groups under 5 URLs unless a URL sits in a money path, and ask for my key paths if I have not listed them. Rank reasons by URLs lost.

Output a table, max 10 rows, columns: reason, URLs lost this week, URLs gained, example URL, likely trigger (deploy, template change, robots change, or "unknown, needs a look"). If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single reason group to investigate first, no alternatives.
```
