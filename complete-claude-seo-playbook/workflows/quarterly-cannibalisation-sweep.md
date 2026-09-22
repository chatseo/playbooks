# The quarterly cannibalisation sweep

**Area:** Keyword research and clustering · **Cadence:** quarterly · **Time:** 2 h

**Trigger.** Every quarter, or right after a batch of new pages goes live on topics you already covered.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Export the Search Console performance report by query and page for the last 3 months. Keep queries with at least 50 impressions in the CSV. | manual | A query by page CSV with clicks, impressions and position. |
| 2 | Paste the export and ask which page Google serves per query, and where the served page changed within the period. | `query-to-page-map` | A map of query to served page, with unstable queries flagged. |
| 3 | Hand it the unstable queries and the pages involved. Ask for the queries where two or more of your pages alternate and the clicks each page gets. | `cannibalisation-finder` | A table of cannibalised queries, competing URLs and a suggested winner. |
| 4 | Decide per cluster: merge the loser into the winner and 301 it, or rewrite the loser to a clearly different intent. Do not leave both as is. | manual | A list of merges with redirects and a list of rewrites. |
| 5 | Ship the redirects and the rewrites in the CMS, then re-export the same report in 28 days and rerun the map to confirm one page per query. | manual | A before and after position for each resolved query. |

**Result.** One page per contested query, a short redirect list executed in the CMS, and a 28-day before and after table that tells you whether the merge recovered the position.
