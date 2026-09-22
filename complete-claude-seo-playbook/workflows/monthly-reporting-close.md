# The monthly reporting close

**Area:** Google Search Console analysis · **Cadence:** monthly · **Time:** 60 min

**Trigger.** The third working day of the month, once the previous month's Search Console data is complete.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Export Search Console pages and queries for last month compared with the month before, and GA4 organic sessions and conversions for the same two periods. | manual | Four exports: two Search Console, two GA4. |
| 2 | Paste the page comparison. Ask for the pages that lost the most clicks with stable or rising impressions, and the ones that gained the most. | `decay-detector` | Two lists: top 10 losers and top 10 gainers with deltas. |
| 3 | Paste all four exports plus the losers and gainers lists and the list of what shipped last month. Ask for the report, with any metric it cannot compute from this data left blank. | `monthly-report` | A one-page report: totals, movers, what shipped, what to do next. |
| 4 | Read every number against the exports, fill the blanks yourself or delete them, then send the report and file the exports in the month's folder. | manual | A sent report and archived exports. |

**Result.** A one-page monthly report built only from exports you checked, with the month's losers feeding the decay rescue and the gainers feeding next month's quick-win round.
