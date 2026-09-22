# Plan the rewrite of a decaying page

**Area:** Content strategy and briefs · **Time:** 45 min · **Skill:** `content-refresh`

**Goal.** Build a section-by-section rewrite plan for one page whose traffic has dropped, based on what it lost and who took it.

**When.** A page that used to bring steady clicks has lost a third or more of them over the last 6 months.

## You need

- a Search Console export for the page, Queries tab, comparing the last 3 months to the same 3 months a year earlier
- the page's current content, pasted in full
- the current top 3 results for its main query, with their headings

## Steps

1. In the export, sort by click difference and keep the queries that lost the most clicks, and separately the queries that gained, so you see what moved.
2. Paste the two lists, the page content and the competitor headings into Claude and ask which sections of your page served the lost queries.
3. Ask Claude to produce a plan with one line per section: keep, rewrite, add or cut, with the query each change serves and what the top 3 do that you do not.
4. Claude returns the plan plus a list of facts and dates in the page that look stale and need checking, without guessing their new values.
5. Approve the plan, update the stale facts from your own sources, and schedule the rewrite with a re-check of the query export 6 weeks after publishing.

**Done when a rewrite plan exists with one action per section and a 6-week check date is on the calendar.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
