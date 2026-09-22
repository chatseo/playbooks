# Catch traffic decay early

**Area:** Google Search Console analysis · **Time:** 30 min · **Skill:** `decay-detector`

**Goal.** Spot pages whose clicks are sliding month over month before the drop shows up in the total, and pick the ones to refresh.

**When.** You run this monthly, or when total clicks dipped and nobody knows which pages did it.

## You need

- a Search Console Pages export comparing the last 28 days to the previous 28 days, with clicks and impressions for both periods
- the same comparison for 3 months ago, so a one-off dip and a trend look different
- publish or last-updated dates per page, from the CMS

## Steps

1. In the comparison export, compute the click difference and the percentage change per page, and keep pages that lost at least 20 percent and at least 30 clicks.
2. Join the 3-month comparison so each page has two consecutive changes, and keep pages that dropped in both periods, which separates decay from noise.
3. Paste the list with last-updated dates into Claude and ask it to sort by clicks lost and to tag each page as stale by date, seasonal by pattern, or unknown.
4. Claude returns the sorted table with the tag and, for stale pages, the one refresh action, and writes cannot compute from this data for pages with no date.
5. Put the top 5 stale pages into the refresh queue this month and set a reminder to rerun the export in 28 days.

**Done when five decaying pages are in the refresh queue and the next monthly run is scheduled.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
