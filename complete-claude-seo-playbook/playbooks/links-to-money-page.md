# Point existing pages at a money page

**Area:** Internal linking · **Time:** 30 min · **Skill:** `link-opportunity-finder`

**Goal.** Find the pages on your site that mention the money page's topic but do not link to it, and add a contextual link from each.

**When.** A commercial page ranks on page two and gets few internal links while your blog talks about its topic all the time.

## You need

- the money page URL, its target query and three close variants
- a crawl export with URL, title, H1 and word count, plus the inlinks list for the money page
- a Search Console export for the money page, Queries tab, over 3 months

## Steps

1. Search your site with a crawler custom search or a site search for the target query and its variants, and export the URLs whose body text contains them.
2. Remove from that list every URL that already links to the money page, using the money page's inlinks export.
3. Paste the remaining URLs with their titles into Claude, with the money page's query and its top Search Console queries, and ask it to rank them by topical closeness.
4. Claude returns the ranked pages with, for each, the sentence where the link should go and an anchor built from a query the money page already gets impressions for.
5. Add the top 10 links in the CMS this week, and check the money page's average position for its target query after 4 weeks.

**Done when ten new contextual links point to the money page from relevant pages, with descriptive anchors.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
