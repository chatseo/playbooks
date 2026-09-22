# Find and resolve cannibalising pages

**Area:** Keyword research and clustering · **Time:** 45 min · **Skill:** `cannibalisation-finder`

**Goal.** Find the queries where two or more of your pages compete against each other, and decide one winner per query.

**When.** Rankings for a target query flip between two of your URLs from week to week, or both sit outside the top 10.

## You need

- a 3-month Search Console export with query, page, clicks, impressions and position (use the API, Looker Studio or a connector so you get query and page together)
- your list of target queries with the page each one is meant to rank

## Steps

1. In the export, keep only queries that appear with two or more different pages, each with at least 50 impressions, so single-page and trivial cases are out.
2. Paste those rows into Claude with your target query-to-page list and ask it to group by query and show every competing page with its clicks, impressions and position.
3. Ask Claude to name, per query, the page with the most clicks as the intended winner, unless your target list names another page, and to flag that conflict explicitly.
4. Claude returns one row per query: winner URL, loser URLs, and one action for each loser, either merge into winner, redirect to winner, or re-target to a different query.
5. Apply the first five actions this week, starting with the queries that have the most impressions, and note the date so you can check positions in 4 weeks.

**Done when every cannibalised query has one named winner and each losing page has one applied action and a check date.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
