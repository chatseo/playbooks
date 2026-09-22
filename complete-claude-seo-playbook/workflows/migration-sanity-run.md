# The migration sanity run

**Area:** Technical SEO and site audits · **Cadence:** once, then after any migration · **Time:** 4 h

**Trigger.** A domain move, a CMS change, a URL structure change or a redesign goes live.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Crawl the new site with Screaming Frog and export all URLs, status codes, redirect targets, canonicals and meta robots. Crawl the old URL list too. | manual | Two crawl exports: old URLs and new site. |
| 2 | Paste the old URL list with the redirect export. Ask for every chain longer than one hop, every loop and every old URL that ends in a 404. | `redirect-chain-map` | A list of redirects to collapse, plus old URLs with no target. |
| 3 | Paste the new crawl's robots.txt, meta robots and canonical columns. Ask for pages that block themselves or canonicalise to the old domain. | `crawl-blockers` | A list of URLs with a self-inflicted block and the fix. |
| 4 | Once the new sitemap is submitted, paste it with the Search Console indexing export a week later. Ask which sitemap URLs are still not indexed. | `sitemap-vs-index` | Unindexed new URLs grouped by reason. |
| 5 | Fix redirects, blocks and sitemap gaps with the developers, recrawl, and keep the three lists until every row is closed. | manual | Three lists closed out, with the recrawl date. |

**Result.** A migration where every old URL lands in one hop, no new page blocks itself and the sitemap matches the index, with the evidence kept for the post-mortem.
