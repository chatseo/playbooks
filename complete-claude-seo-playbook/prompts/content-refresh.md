# Plan the refresh of a decaying page

**Area:** Content strategy and briefs

**When.** Paste this when a page that used to bring traffic has slipped and you need to know what to change, not just that it dropped.

## Prompt

```
Below are: the current text of a page that lost traffic, and its Search Console Queries export for the last 3 months compared with the previous 3 months (query, clicks, impressions, position for both periods). If either is missing, ask me for it before doing anything.

Diagnose first, then plan. Split the loss three ways: queries where position dropped by 3 or more, queries where position held but impressions fell by 30 percent or more (demand or SERP change, not the page), and queries that disappeared. Ignore queries under 20 impressions in both periods. Read the page against the dropped queries: what does it fail to answer, what is stale (dates, prices, versions, screenshots)?

Output: a Diagnosis section (max 5 lines), a table of max 10 queries sorted by clicks lost, columns: query, clicks before, clicks after, position before, position after, cause, then a Refresh plan of max 6 edits naming the section and the change. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single edit to make first, no alternatives.
```
