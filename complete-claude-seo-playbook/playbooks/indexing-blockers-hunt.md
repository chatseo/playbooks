# Find pages blocked from indexing

**Area:** Technical SEO and site audits · **Time:** 45 min · **Skill:** `crawl-blockers`

**Goal.** List every page that should rank but is kept out of the index by robots.txt, a noindex tag or a canonical pointing elsewhere.

**When.** Important pages are missing from search results or Search Console shows a jump in excluded pages.

## You need

- a full crawl export with URL, indexability, indexability status, canonical URL and robots directives columns
- your robots.txt file pasted as text
- the list of URLs that must be indexable, such as products, categories and money pages

## Steps

1. Filter the crawl export to rows marked non-indexable and keep the URL, the indexability status and the canonical column, then export that subset.
2. Paste the subset, the robots.txt and the must-index list into Claude and ask it to match each blocked URL to the rule or tag that blocks it.
3. Ask Claude to separate blocks that look intentional, such as cart and filter pages, from blocks on must-index URLs, and to name the single fix per wrongly blocked URL.
4. Claude returns a table: URL, blocking mechanism, intentional or wrong, and the one fix, such as remove noindex, change canonical, or edit a named robots.txt line.
5. Apply the fixes for the wrongly blocked URLs, then use URL Inspection in Search Console on three of them to confirm they now show as indexable.

**Done when no must-index URL appears as non-indexable in a fresh crawl.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
