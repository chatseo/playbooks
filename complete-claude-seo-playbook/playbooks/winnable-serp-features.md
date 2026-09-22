# Find SERP features you can win

**Area:** Competitor and SERP analysis · **Time:** 45 min · **Skill:** `serp-feature-audit`

**Goal.** List the SERP features on your target queries that a page like yours could realistically take, and the change each one needs.

**When.** You rank in the top 5 for queries where a feature above you takes most of the clicks.

## You need

- your top 50 queries by impressions with position, from a 28-day Search Console Queries export
- for each of those queries, the SERP features present and who holds them, from a rank tracker export or a manual check
- the page ranking for each query, with its headings

## Steps

1. Build a sheet with query, your position, the features present, the holder of each feature, and your page URL, then keep queries where you rank 5 or better.
2. Paste the sheet with your pages' headings into Claude and ask it to name, per feature, what the holder's snippet contains that your page lacks.
3. Ask Claude to rank the features by winnability using only your position and the gap it found, and to mark features like ads or knowledge panels as not winnable by content.
4. Claude returns the ranked list with, per winnable feature, the exact page change: a 40 to 60 word answer paragraph under a matching H2, a table, or a list.
5. Make the top 5 changes, and check the features in your rank tracker or by hand after 3 weeks.

**Done when five feature-targeted page changes are live and a 3-week check is scheduled.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
