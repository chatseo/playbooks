# Reconcile the sitemap with the crawl

**Area:** Technical SEO and site audits

**When.** Paste this with your sitemap URLs and a crawl export when you suspect the sitemap lists pages that should not be there or misses ones that should.

## Prompt

```
Below are: the list of URLs in my XML sitemap, and a Screaming Frog crawl export (Address, Status Code, Indexability, Canonical Link Element) or the Search Console Pages report export. If either is missing, ask me for it before doing anything.

Compare the two sets. Report: sitemap URLs that return non 200, are noindexed, or canonicalise elsewhere (they should leave the sitemap); indexable 200 URLs found in the crawl but absent from the sitemap (they should join it, unless they are parameter or paginated URLs); sitemap URLs never seen in the crawl (orphans, check whether they should exist). Ignore image, PDF and feed URLs. Where the Search Console export is present, add how many sitemap URLs are reported as not indexed and the top reason.

Output three tables, max 15 rows each, columns: URL, issue, evidence (status, directive or canonical target), fix. Then a totals line: sitemap URLs, should leave, should join, orphans. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the one set of URLs to fix in the sitemap first, no alternatives.
```
