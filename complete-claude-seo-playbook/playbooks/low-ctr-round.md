# Run a low-CTR title round

**Area:** Google Search Console analysis · **Time:** 30 min · **Skill:** `low-ctr-finder`

**Goal.** Find the queries where you rank in the top 10 but get far fewer clicks than the position should bring, and fix the snippet.

**When.** Impressions are healthy but clicks are flat, or a page ranks well and nobody clicks it.

## You need

- a 28-day Search Console export, Queries tab, with CTR and position
- your own site's CTR by position, computed from the same export as the median CTR at each rounded position
- the title and meta description of the page ranking for each low-CTR query

## Steps

1. In a sheet, round position to the nearest whole number and compute the median CTR per position for rows with at least 100 impressions, which is your own benchmark.
2. Keep rows with position 10 or better whose CTR is under half the benchmark for their position, and sort by impressions descending, keeping the top 25.
3. Paste the 25 rows with each page's title and description into Claude, with the benchmark table, and ask it to explain the gap per row from the snippet alone.
4. Claude returns per row: the likely snippet problem, a rewritten title under 60 characters, a rewritten description, or SERP feature likely if the snippet already matches the query.
5. Ship the rewrites for the rows not marked SERP feature likely, and re-export CTR for those queries in 4 weeks against the same benchmark.

**Done when every low-CTR query has a new snippet live or a SERP feature note, and a 4-week check is scheduled.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
