# Fix a page's heading hierarchy

**Area:** On-page optimization · **Time:** 20 min · **Skill:** `heading-structure-fix`

**Goal.** Repair a page whose headings skip levels, repeat the H1 or use headings for styling so the structure reads as an outline.

**When.** A crawl flags multiple H1s, missing H1 or H3s without a parent H2 on an important page.

## You need

- the page's headings in order with their level, exported from your crawler or copied from the page source
- the page's target query and one-line purpose

## Steps

1. Copy the heading list with levels into a text file, keeping the order exactly as it appears in the HTML, including headings used for buttons or sidebars.
2. Paste the file and the target query into Claude and ask it to list every violation: multiple H1s, skipped levels, headings that are not section titles, and empty headings.
3. Ask Claude to propose the corrected outline with one H1 containing the query's main words, H2s for main sections and H3s only under a parent H2.
4. Claude returns a before and after table, one row per heading, with the action for each: keep, change level, rewrite text or convert to styled paragraph.
5. Apply the table in the CMS, then recrawl the single URL to confirm exactly one H1 and no skipped levels remain.

**Done when a recrawl of the page shows one H1 and every H3 sits under an H2.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
