# Find sitemap URLs Google skipped

**Area:** Technical SEO and site audits · **Time:** 45 min · **Skill:** `sitemap-vs-index`

**Goal.** List the URLs in your sitemap that Google has not indexed, sorted by the reason, and decide what to do with each group.

**When.** The Sitemaps report shows many more discovered URLs than indexed ones.

## You need

- your sitemap URLs as a list, fetched from the sitemap files
- the Pages report export from Search Console filtered to the sitemap, with the reason per not-indexed URL
- a crawl export with word count, canonical and internal link count per URL

## Steps

1. Export the not-indexed URLs from the Pages report filtered to your sitemap, keeping the reason column, and join them to the crawl export on URL.
2. Paste the joined table into Claude and ask it to group the URLs by reason and by URL pattern, and to summarise the word count and inlink count of each group from the columns given.
3. Ask Claude to assign one action per group: improve content, add internal links, remove from sitemap, fix canonical, or wait, based only on the reason and the crawl columns.
4. Claude returns the groups with counts, the one action each, and marks groups where the crawl data is missing as cannot compute from this data.
5. Remove the remove-from-sitemap groups first, apply the other actions to the largest group, and re-export the report in 3 weeks.

**Done when every not-indexed sitemap URL sits in a group with one action, and the sitemap no longer lists pages you do not want indexed.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
