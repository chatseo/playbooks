# Explain what changed in index coverage this week

**Area:** Technical SEO and site audits · **Time:** 30 min · **Skill:** `index-coverage-diff`

**Goal.** Turn two weekly snapshots of the Search Console Pages report into a plain explanation of what moved and whether it matters.

**When.** The indexed page count moved noticeably this week and someone wants to know why.

## You need

- last week's and this week's export of the Pages report in Search Console, with the reason and the count per reason
- the URL list for the two reasons that changed the most, exported from the report
- a note of what shipped on the site this week, deploys, redirects, new sections

## Steps

1. Put both exports side by side in a sheet, one row per reason, and add a column with the difference in count so the biggest movers are obvious.
2. Export the URL lists for the two reasons with the largest change and paste them into Claude with the diff sheet and the note of what shipped.
3. Ask Claude to describe what kind of URLs moved, by folder or pattern, and to link each movement to a shipped change where the note supports it.
4. Claude returns a short summary per moved reason: the pattern, the likely trigger from your notes or unknown, and whether it needs action or is expected.
5. For each movement marked needs action, open one ticket naming the pattern and the reason, and file the summary so next week's diff has a baseline.

**Done when each reason that moved has a written explanation and any harmful movement has a ticket.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
