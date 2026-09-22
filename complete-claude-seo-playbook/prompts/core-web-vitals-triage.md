# Triage Core Web Vitals by traffic

**Area:** Technical SEO and site audits

**When.** Paste this with field data and traffic per URL when the vitals report is red and you need to know where to start.

## Prompt

```
Below are: 75th percentile field data (LCP, INP, CLS from PageSpeed Insights or the Search Console Core Web Vitals report) per URL or URL group, and sessions or clicks per URL from GA4 or Search Console for the last 28 days. If the traffic numbers are missing, ask me for them before doing anything.

Triage by traffic, not by score. A URL fails when LCP is above 2.5 seconds, INP above 200 milliseconds, or CLS above 0.1. Group failing URLs by template (product, category, article, home) when paths make it obvious. Rank groups by traffic on failing URLs. For each group say which metric fails and which is within 20 percent of its threshold, the cheapest win. Name causes only if I pasted lab diagnostics; otherwise write "needs lab data".

Output a table, max 10 rows, columns: template or URL, URLs failing, traffic on failing URLs, failing metric, value, distance to threshold, likely cause. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single template and metric to fix first, no alternatives.
```
