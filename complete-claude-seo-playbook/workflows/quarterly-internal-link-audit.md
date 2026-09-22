# The quarterly internal link audit

**Area:** Internal linking · **Cadence:** quarterly · **Time:** 3 h

**Trigger.** Every quarter, or after 20 or more pages have been added since the last audit.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Crawl the site with Screaming Frog and export all internal links with source, target, anchor text and crawl depth. Export the sitemap URL list too. | manual | An internal links export and a sitemap URL list. |
| 2 | Paste the sitemap list and the links export. Ask for sitemap URLs with zero internal links pointing to them. | `orphan-finder` | A list of orphan URLs with a suggested parent page each. |
| 3 | Paste the crawl depth column. Ask for pages deeper than 3 clicks that get Search Console impressions, and the shortest path that would fix each. | `link-depth-fix` | A list of deep pages with one link to add per page. |
| 4 | Paste the anchor text column for your 10 most important pages. Ask for anchors that are generic, repeated verbatim, or off topic. | `anchor-text-audit` | Per money page, the anchors to rewrite and a replacement each. |
| 5 | Add the orphan links, the depth links and the anchor rewrites in the CMS, working page by page from the three lists. | manual | Three lists closed with a ship date. |

**Result.** No orphan in the sitemap, no page with impressions deeper than 3 clicks, and descriptive anchors on the money pages, all done from one crawl export.
