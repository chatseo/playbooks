# Find the keywords a competitor owns and you miss

**Area:** Keyword research and clustering · **Time:** 1 h · **Skill:** `keyword-gap`

**Goal.** Get a short, ranked list of keywords one competitor ranks for that you are missing, filtered to what your site can realistically win.

**When.** A competitor keeps showing up above you and you want their list, not a guess about it.

## You need

- a keyword gap or content gap export from Ahrefs or Semrush for one competitor versus your domain
- a one-paragraph description of what your site sells and what it will never write about

## Steps

1. Run the gap report with your domain as the target and one competitor, export it, and keep the keyword, volume, difficulty and competitor position columns.
2. Delete rows where the competitor ranks worse than position 20, and rows for their brand name, so you are left with keywords they actually own.
3. Paste the remaining rows into Claude with your site description and ask it to drop any keyword your site would not credibly serve, giving a one-line reason for each drop.
4. Claude returns the kept keywords grouped by the page type you would need, a blog post, a comparison page or a product page, with volume and difficulty copied from the export.
5. Pick the ten kept keywords with the lowest difficulty above 200 monthly searches and add each to your backlog with its page type.

**Done when ten gap keywords sit in your backlog, each with a page type and the competitor URL to beat.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
