# Produce the monthly client report

**Area:** Google Search Console analysis · **Time:** 45 min · **Skill:** `monthly-report`

**Goal.** Write a one-page monthly SEO report that says what changed, why, and what happens next, in words a client will read.

**When.** It is the first week of the month and the report is due.

## You need

- a Search Console Performance export comparing last month to the previous month and to the same month last year, at site level and by page
- GA4 organic sessions and conversions for the same periods, exported as a table
- the list of work shipped last month with dates

## Steps

1. Export the three comparisons and the GA4 table, and write the shipped-work list as dates and one line each, so Claude can connect changes to results.
2. Paste everything into Claude and ask for a report in four blocks: the headline numbers with both comparisons, the three pages that moved most, what shipped and its visible effect, next month's plan.
3. Tell Claude to use only numbers in the exports, to say cannot compute from this data where a figure is missing, and to keep the whole report under 400 words.
4. Claude returns the report with each claim tied to a number from the exports and a plain-language sentence on what it means for the client.
5. Read it once as the client would, cut any sentence that needs SEO knowledge to understand, and send it with the exports attached.

**Done when a report under 400 words with four blocks has been sent, with every number traceable to an export.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
