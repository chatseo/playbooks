# Find striking distance pages

**Area:** Google Search Console analysis

**When.** Paste this with a queries export when you want the pages one push away from page one clicks.

## Prompt

```
Below is my Search Console export for the last 3 months with query and page dimensions, columns query, page, clicks, impressions, CTR, position, plus my brand terms. If the export or the brand terms are missing, ask me to paste them before doing anything.

Find striking distance queries: average position between 8 and 15, at least 100 impressions, not a brand query. Rank by the clicks gained if the query moved to position 5, using a CTR of 6 percent at position 5, and state that assumption in the output. Group queries by page so I see each page's total opportunity. Note when a page has 3 or more striking distance queries, since one improvement lifts them all.

Output a table, max 15 rows, one per page, columns: page, striking distance queries (count), top query, impressions total, position of the top query, projected clicks at position 5, what the page is missing versus the query (one line). If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single page to work on this week, no alternatives.
```
