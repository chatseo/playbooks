---
name: crawl-blockers
description: Find pages blocked from indexing by robots.txt, noindex, or canonical conflicts. Use for a technical audit or when pages are missing from Google.
---

Pull every indexable URL from the sitemap. For each, check: robots.txt disallow, meta robots noindex, canonical pointing elsewhere, and GSC coverage state.
Report ONLY conflicts — a URL that is submitted but blocked, or canonicalised to a page that is itself noindexed.
Columns: URL | blocker | where it is set | traffic at stake (GSC clicks, last 28d).
Cap at 20 rows, sorted by clicks lost.
End with the single blocker fix that unlocks the most traffic.
