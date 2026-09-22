# Find and rescue orphan pages

**Area:** Internal linking · **Time:** 45 min · **Skill:** `orphan-finder`

**Goal.** Find pages that exist but receive no internal links, and give each one a link from a relevant page or a decision to remove it.

**When.** Your sitemap or CMS has far more URLs than your crawl finds, or you suspect old pages are unreachable.

## You need

- the full URL list from your sitemap or CMS export
- the crawl export from a crawl started at the homepage, with the inlinks count column
- a 3-month Search Console Pages export, so orphans that still get traffic are visible

## Steps

1. Compare the sitemap list against the crawled URL list and keep every URL that is in the sitemap but not in the crawl, or has zero inlinks in the crawl.
2. Join that list to the Search Console export on URL so each orphan carries its clicks and impressions, and sort by impressions descending.
3. Paste the list into Claude with your site's main section names and ask it to propose, per orphan, one existing page that should link to it and a suggested anchor.
4. Claude returns URL, impressions, the proposed linking page, the anchor, or remove if the page has no traffic and no purpose it can see, with a reason.
5. Add the links for every orphan with impressions, decide on each remove suggestion yourself, and recrawl to confirm no page shows zero inlinks.

**Done when every orphan with impressions has at least one internal link and the rest have a keep or remove decision.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
