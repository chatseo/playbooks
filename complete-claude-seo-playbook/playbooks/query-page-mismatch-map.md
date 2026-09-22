# Map queries to the page Google serves

**Area:** Google Search Console analysis · **Time:** 30 min · **Skill:** `query-to-page-map`

**Goal.** See which page Google actually shows for each of your target queries, and fix every case where it is not the page you built.

**When.** You have a target keyword map and want to know how far reality is from it.

## You need

- your target keyword map: query and intended URL, one row per query
- a 3-month Search Console export with both query and page dimensions, from the API, Looker Studio or a connector

## Steps

1. Filter the export to your target queries and, for each query, keep the page with the most impressions as the served page.
2. Put the intended URL and the served URL side by side per query and mark every row where they differ.
3. Paste the mismatched rows into Claude with the titles of both pages per row and ask it to explain, from the titles and the query, why the served page wins.
4. Claude returns per query: the mismatch reason, and one action, either strengthen the intended page for the query, redirect the served page, or update the map to the served page.
5. Apply the update-the-map actions today, queue the strengthen actions by impressions, and treat the redirect actions as decisions to confirm before touching anything.

**Done when every target query has either a matching served page or one queued action to close the gap.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
