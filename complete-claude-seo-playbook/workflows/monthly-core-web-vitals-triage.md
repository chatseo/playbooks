# The monthly Core Web Vitals triage

**Area:** Technical SEO and site audits · **Cadence:** monthly · **Time:** 90 min

**Trigger.** Mid-month, when the Search Console Core Web Vitals report has a full 28 days of field data.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Export the Search Console Core Web Vitals report for mobile and desktop, and the performance report by page for the same 28 days. | manual | A CWV export by URL group and a clicks by page export. |
| 2 | Paste both exports. Ask for the failing URL groups ranked by the clicks they carry. If the clicks export is missing, it says the ranking cannot be computed from this data. | `core-web-vitals-triage` | Failing groups ranked by traffic at risk, with the failing metric. |
| 3 | Run the top 5 URLs through PageSpeed Insights, paste the diagnostics, and ask which single fix per template covers the most URLs. | `core-web-vitals-triage` | One fix per template with the URLs it covers. |
| 4 | Open one developer ticket per template fix with the URL list and the metric, and note the current field value. | manual | Tickets with a baseline value each. |
| 5 | Next month, paste the new CWV export with the ticket list. Ask for the before and after per template for the month's report. | `monthly-report` | A CWV section for the monthly report. |

**Result.** Failing templates ranked by the traffic they put at risk, one ticket per template, and a before and after line that lands in next month's report.
