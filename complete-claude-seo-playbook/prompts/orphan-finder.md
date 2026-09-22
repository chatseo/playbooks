# Find orphan and near orphan pages

**Area:** Internal linking

**When.** Paste this with a crawl export and your sitemap when pages exist but nothing on the site links to them.

## Prompt

```
Below are: a Screaming Frog crawl export with Address, Status Code, Indexability, Inlinks and Crawl Depth; my XML sitemap URL list; and, if I have it, a Search Console Pages export for the last 3 months. If the crawl or the sitemap is missing, ask me for it before doing anything.

Find orphans and near orphans. Orphan: an indexable 200 URL in the sitemap or in Search Console with 0 inlinks in the crawl. Near orphan: 1 to 2 inlinks, or inlinks only from paginated, tag or footer pages. Exclude legal pages, author pages and URLs with parameters. Rank by impressions if given, otherwise by whether the URL sits in a money path (ask for my key paths if needed).

Output a table, max 20 rows, columns: URL, inlinks, crawl depth, impressions, type (orphan, near orphan), suggested linking page (a topically close crawl page with at least 5 inlinks), proposed anchor. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single orphan to link first and from where, no alternatives.
```
