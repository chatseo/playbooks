# The weekly index health check

**Area:** Technical SEO and site audits · **Cadence:** weekly · **Time:** 40 min

**Trigger.** Every Monday morning, before any release goes out that week.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Export the Search Console Pages indexing report and keep last week's export next to it. Paste both. | `index-coverage-diff` | A diff: URLs that became not indexed, new reasons, and counts per reason. |
| 2 | Paste your sitemap URL list and the same indexing export. Ask which sitemap URLs are not indexed and the reason Search Console gives per URL. | `sitemap-vs-index` | A list of unindexed sitemap URLs grouped by reason. |
| 3 | For the URLs newly dropped this week, paste their robots.txt rules, meta robots and canonical tags. Ask which of them conflict. | `crawl-blockers` | Per URL, the blocking rule and the fix. |
| 4 | Open one ticket per fix with the URL list attached. Anything without a clear cause goes on a watch list for next Monday. | manual | Tickets filed and a watch list of unexplained drops. |

**Result.** A weekly diff of what left the index and why, with fixes ticketed before the next release and a watch list that catches slow leaks.
