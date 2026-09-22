# Map keywords to buying stages

**Area:** Competitor and SERP analysis

**When.** Paste this with a keyword list and your current pages when you want to see which stage of the funnel has no page.

## Prompt

```
Below is a keyword list with volume and my current page for each if any, plus one line on what I sell and who buys it. If either is missing, ask me for it before doing anything.

Map each keyword to a buying stage: problem aware (names a pain, not a solution), solution aware (names a category or approach), product aware (names a product, a comparison, or a brand plus modifier), ready to buy (pricing, trial, buy, discount, near me, a plan name). Then check coverage: which stages have pages, which have volume but no page, and which have a page in the wrong format (a pricing query landing on a blog post). Sum volume per stage from the input only.

Output a table, max 40 rows, columns: keyword, volume, stage, my page (or none), fit (fits, wrong format, missing). Then a stage summary: stage, keyword count, summed volume, pages, gap. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single stage to build for first and the page type, no alternatives.
```
