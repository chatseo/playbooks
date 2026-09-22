# The monthly quick-win round

**Area:** Google Search Console analysis · **Cadence:** monthly · **Time:** 45 min

**Trigger.** Day 1 of the month, with the last 28 days of Search Console data exported by page and query.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Export the Search Console performance report by query with page for 28 days. Paste it and ask for queries at position 8 to 15 with the most impressions. | `position-8-15-finder` | A table of 10 queries with page, position, impressions and clicks. |
| 2 | Paste the pages from that table. Ask which of them also sit below the expected CTR for their position. | `low-ctr-finder` | The subset of pages where a title change would count twice. |
| 3 | For each page in the subset, paste the current title and the target query. Ask for two title options that state the answer the query wants. | `title-rewriter` | Two titles per page. |
| 4 | Ship one title per page in the CMS, and add a paragraph answering the query near the top if the page does not already. | manual | Changed pages with a ship date. |
| 5 | In 28 days, re-export the same report and compare position and CTR per query. Keep what moved up, revert what fell. | manual | Per query, before and after position and CTR. |

**Result.** Ten queries a month pushed from page two toward page one with title and answer changes, and a dated table that tells you which ones moved.
