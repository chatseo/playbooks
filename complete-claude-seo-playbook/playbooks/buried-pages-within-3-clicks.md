# Pull buried pages within 3 clicks

**Area:** Internal linking · **Time:** 45 min · **Skill:** `link-depth-fix`

**Goal.** Find pages more than 3 clicks from the homepage that earn impressions, and bring each within 3 clicks with one added link.

**When.** Your crawl depth report shows a long tail of pages at depth 4 and beyond.

## You need

- a crawl export from the homepage with the crawl depth column
- a 3-month Search Console Pages export with impressions per URL
- your navigation structure: which categories and hub pages sit at depth 1 and 2

## Steps

1. Filter the crawl export to depth greater than 3, join it to the Search Console export on URL, and sort by impressions descending.
2. Take the top 30 by impressions and paste them into Claude with the list of depth 1 and depth 2 pages and their topics.
3. Ask Claude to assign each buried page to the one depth 2 page whose topic fits best, and to write the anchor that page should use.
4. Claude returns buried URL, impressions, current depth, the depth 2 page to link from, the anchor, and flags pages it cannot place in any existing section.
5. Add the links, decide whether unplaced pages need a new section or removal, and recrawl to confirm the 30 pages now sit at depth 3 or less.

**Done when the top 30 buried pages by impressions show a crawl depth of 3 or less in a fresh crawl.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
