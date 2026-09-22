# Write missing meta descriptions in batch

**Area:** On-page optimization · **Time:** 1 h · **Skill:** `meta-description-batch`

**Goal.** Fill every missing or weak meta description on the pages that get impressions, in one sitting, without generic copy.

**When.** Your crawl shows dozens of pages with no meta description or a duplicated one.

## You need

- a crawler export (Screaming Frog or similar) with URL, title, meta description and its length
- a 28-day Search Console export, Pages tab, so you can prioritise by impressions
- the first 200 words of each page you are fixing, or the page's H1 and H2s

## Steps

1. Join the two exports on URL, keep rows where the description is empty, duplicated or under 70 characters, and sort by impressions descending.
2. Take the top 30 rows and paste them into Claude with each page's H1, H2s and opening paragraph, in batches of 10.
3. Ask Claude to write one description per page between 120 and 155 characters, stating what the page gives and to whom, using only what the page actually says.
4. Claude returns URL, new description and character count, and flags pages where the content was too thin to describe honestly.
5. Paste the descriptions into the CMS, and treat every flagged page as a content problem to fix rather than a description to fake.

**Done when the top 30 pages by impressions each have a unique description of 120 to 155 characters live.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
