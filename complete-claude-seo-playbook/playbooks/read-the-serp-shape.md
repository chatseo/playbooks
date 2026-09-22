# Read which format ranks for a keyword

**Area:** Competitor and SERP analysis · **Time:** 20 min · **Skill:** `serp-shape-reader`

**Goal.** Decide the content format for one keyword by reading what the top 10 actually are, not what you would like to write.

**When.** You are about to brief a page and are not sure whether it should be a guide, a list, a tool or a product page.

## You need

- the keyword
- for each of the top 10 results: URL, title, page type as you see it, word count if your tool gives it, and any SERP features present

## Steps

1. Search the keyword in a private window, and for each of the top 10 write the URL, the title, what kind of page it is, and note every SERP feature on the page.
2. Paste the 10 rows and the features into Claude and ask it to count the formats and name the dominant one, and to note any format that appears only once.
3. Ask Claude to state the one format you should build and the one feature you could target, based only on the counts, and to say mixed if no format has a majority.
4. Claude returns the format decision with the count behind it, the outlier formats, and the feature to target with the result that currently holds it.
5. Write the format decision at the top of the brief, and if the answer was mixed, pick the format closest to your site's strength and note the risk.

**Done when the brief states one format with the SERP count that justifies it.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
