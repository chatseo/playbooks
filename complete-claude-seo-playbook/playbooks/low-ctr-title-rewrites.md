# Rewrite titles for pages ranking well with poor CTR

**Area:** On-page optimization · **Time:** 45 min · **Skill:** `title-rewriter`

**Goal.** Rewrite the titles of pages that already rank in the top 5 but get fewer clicks than their position deserves.

**When.** You have pages sitting at position 1 to 5 whose CTR is well under what the position usually brings.

## You need

- a 28-day Search Console export, Pages tab, with clicks, impressions, CTR and position
- the current title tag of each page, from your crawler or the CMS
- the top query for each of those pages, from the Queries tab filtered by page

## Steps

1. In the export, keep pages with average position under 5 and at least 500 impressions, then sort by CTR ascending and take the bottom 20.
2. Paste those 20 rows with their current titles and top query into Claude and ask it to explain, per page, why the title may be losing the click against the query.
3. Ask Claude to write three title options per page under 60 characters, each leading with the query's main words, and to pick one with a one-line reason.
4. Claude returns one recommended title per page with the reason, and marks pages where the low CTR is more likely a SERP feature issue than a title issue.
5. Change only the recommended titles, note the date, and compare CTR for those pages against the 28 days before the change after 4 weeks.

**Done when the 20 pages have new titles live and a dated note exists to compare CTR in 4 weeks.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
