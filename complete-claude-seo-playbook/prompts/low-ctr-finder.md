# Find top 10 queries with weak CTR

**Area:** Google Search Console analysis

**When.** Paste this with a queries export when rankings look fine but clicks do not follow.

## Prompt

```
Below is my Search Console Queries export for the last 28 days (query, clicks, impressions, CTR, position) and my brand terms. If either is missing, ask me for it before doing anything.

Find queries in the top 10 where CTR sits below the position's expected curve. Use this curve unless I give my own: position 1, 25 percent; 2, 15; 3, 10; 4, 7; 5, 6; 6 to 10, 3. Keep queries with position 10 or better and at least 100 impressions. Exclude brand queries. Exclude queries where the SERP probably answers above the results (the query reads as a definition, a number, a date, a unit conversion) and list those separately with a note. Rank by impressions multiplied by the CTR gap in points.

Output a table, max 15 rows, columns: query, impressions, position, CTR, expected CTR, missed clicks (impressions times gap), page, likely cause (title, snippet, SERP feature, intent mismatch). If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single query and page to fix first and which element, no alternatives.
```
