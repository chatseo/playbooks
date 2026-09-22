# Audit internal anchor text

**Area:** Internal linking · **Time:** 45 min · **Skill:** `anchor-text-audit`

**Goal.** Find internal anchors that are either vague, such as click here, or repeated exact-match for one page, and rewrite the worst.

**When.** You have never reviewed anchors, or a page gets hundreds of identical exact-match internal anchors.

## You need

- an internal links export from your crawler with source URL, destination URL and anchor text
- the list of your 20 most important destination pages with their target query

## Steps

1. Filter the inlinks export to the 20 destination pages and count, per destination, how many distinct anchors point to it and how often each one repeats.
2. Paste the counts and the anchors into Claude with each page's target query and ask it to flag vague anchors and any single anchor above half of a page's inlinks.
3. Ask Claude to propose replacements for the vague anchors and a spread of natural variants for the over-repeated ones, each variant describing the destination.
4. Claude returns source URL, destination, current anchor, new anchor, and the reason, and leaves anchors that already describe the destination untouched.
5. Apply the changes for the top 5 destination pages first, since those carry the most weight, and rerun the count after the next crawl.

**Done when no top-20 page has a single anchor above half its inlinks and vague anchors to those pages are gone.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
