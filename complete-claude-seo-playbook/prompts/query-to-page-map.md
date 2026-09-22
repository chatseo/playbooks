# Map queries to their owning page

**Area:** Google Search Console analysis

**When.** Paste this with a combined query and page export when you want to know which page owns which query and where the conflicts are.

## Prompt

```
Below is my Search Console export with both query and page dimensions for the last 3 months (query, page, clicks, impressions, position), plus my brand terms. If the export has only queries or only pages, ask me for the combined one before doing anything.

Build the query to page map. For each query with at least 50 impressions, name the page that should own it: the page with the most clicks when it also holds the best position, otherwise flag a conflict. Then, for each owning page, list its query set and mark queries that do not fit the page's topic (the page ranks by accident). Mark queries with no page at position 20 or better as unowned. Skip brand queries.

Output a table, max 25 rows, columns: query, impressions, owning page, position, status (owned, conflict, misfit, unowned), action (keep, consolidate, add a section, new page). Then a count per status. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single conflict or unowned query to resolve first, no alternatives.
```
