# Find pages cannibalising each other

**Area:** Keyword research and clustering

**When.** Paste this when two of your pages seem to trade places for the same queries and you need to know which one should win.

## Prompt

```
Below is my Search Console export for the last 3 months with one row per query and page pair, columns query, page, clicks, impressions, CTR, position, plus my brand terms. If the export or the brand terms are missing, ask me to paste them before doing anything.

Find cannibalisation: queries where two or more of my pages each have at least 50 impressions. Exclude brand queries. Exclude queries under 100 total impressions. For each query, name the page with the most clicks as the leader and the others as competitors. Mark the case serious when the leader holds under 60 percent of the query's clicks or when the pages sit within 3 positions of each other.

Output a table, max 15 rows, sorted by total impressions descending, columns: query, total impressions, leader page, competitor pages, leader click share, severity (serious or minor), fix (consolidate, redirect, differentiate intent, or canonical). If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single query to fix first and which fix, no alternatives.
```
