# Find pages ranking for the wrong intent

**Area:** Competitor and SERP analysis · **Time:** 45 min · **Skill:** `intent-mismatch`

**Goal.** Find your pages that get impressions for queries they were never built to answer, and decide whether to serve or release each query.

**When.** A page gets lots of impressions with low CTR and a poor position, and its queries look unrelated.

## You need

- a 3-month Search Console export with query and page together, from the API or a connector
- each page's stated purpose in one line, from your keyword map or the H1

## Steps

1. For each page, keep its top 20 queries by impressions and paste them into Claude with the page's one-line purpose, in batches of 10 pages.
2. Ask Claude to tag each query as matched to the purpose, adjacent, or mismatched, and to state the intent the mismatched query actually carries.
3. Claude returns per page the mismatched queries with their impressions, position and the intent they carry, and skips pages where everything matched.
4. For each page with mismatched queries above 500 impressions total, decide one thing: build a new page for that intent or add a short section that serves it.
5. Add the build decisions to the backlog with the impressions as the priority score, and write the sections for the add decisions this week.

**Done when every page with material mismatched impressions has either a new page in the backlog or a new section live.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
