# The quarterly intent mismatch audit

**Area:** Competitor and SERP analysis · **Cadence:** quarterly · **Time:** 2 h

**Trigger.** Every quarter, on pages that rank for queries they were never built to answer.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Export Search Console queries with page for 3 months. Keep pages with at least 100 impressions in the CSV and paste it with a one-line purpose per page. | `intent-mismatch` | Pages whose top queries ask for something else, with the mismatched queries listed. |
| 2 | Paste the mismatched queries. Ask for the buying stage of each and whether a page for that stage already exists on the site. | `buying-stage-mapper` | Per query, a stage and an existing page or a gap. |
| 3 | For pages with a fixable mismatch, paste the page text and the mismatched queries. Ask for a rewrite plan that serves both intents or splits them. | `content-refresh` | A rewrite or split plan per page. |
| 4 | Ship the rewrites, create the split pages for the gaps, and add the new pages to the linking queue. | manual | Rewritten pages and new pages queued for links. |
| 5 | In 28 days, re-export the query by page report and check that the mismatched queries now land on the intended page. | manual | Per query, the page served before and after. |

**Result.** Queries that landed on the wrong page now reach a page built for their stage, and the gaps became new pages instead of a dead end in the funnel.
