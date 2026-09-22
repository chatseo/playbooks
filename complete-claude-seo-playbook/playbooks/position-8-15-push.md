# Push pages stuck at 8-15

**Area:** Google Search Console analysis · **Time:** 20 min · **Skill:** `position-8-15-finder`

**Goal.** Find the queries where you sit just below the top results with real impressions, and give each one a single push.

**When.** You want quick wins from pages that are already close rather than new content.

## You need

- a 28-day Search Console export, Queries tab, with clicks, impressions, CTR and position
- the page ranking for each of those queries, from the Pages tab with the query filter, or from an API pull with both dimensions

## Steps

1. In the export, keep rows with average position between 8 and 15 and at least 200 impressions, then sort by impressions descending and take the top 30.
2. Add the ranking page for each query, then paste the 30 rows into Claude with each page's title and H2s.
3. Ask Claude to say, per query, whether the query's main words appear in the title, an H2 and the first paragraph, and to name the one missing element.
4. Claude returns query, page, position, the one gap, and the one fix: a title edit, a new H2 section, or an internal link from a named stronger page.
5. Apply the fix for the 10 queries with the most impressions, note the date, and compare position for those queries after 4 weeks.

**Done when ten queries have one applied fix each and a dated note to compare position in 4 weeks.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
