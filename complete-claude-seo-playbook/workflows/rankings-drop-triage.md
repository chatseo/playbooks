# The rankings drop triage

**Area:** Google Search Console analysis · **Cadence:** when rankings drop · **Time:** 60 min

**Trigger.** Clicks or average position fall by 20 percent or more week over week on a page that matters.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Export Search Console pages and queries for the last 7 days compared with the previous 7, plus the Pages indexing report. Paste the indexing report with last week's. | `index-coverage-diff` | Whether the affected URLs left the index, and the reason if they did. |
| 2 | If still indexed, paste the query by page comparison. Ask whether Google swapped which of your pages it serves for the dropped queries. | `query-to-page-map` | Per dropped query, the page served before and after. |
| 3 | If the page did not change, paste the current top 10 for the main query. Ask whether the SERP now wants a different intent or format than your page. | `intent-mismatch` | A verdict: intent shift, format shift, or neither. |
| 4 | Decide the lane: indexing fix, cannibalisation sweep, decay rescue, or wait one more week if nothing explains it. Write the decision and the date down. | manual | One named next workflow, or a dated wait. |

**Result.** Within an hour of a drop you know whether it is indexing, a page swap, a SERP shift or noise, and which workflow takes it from there.
