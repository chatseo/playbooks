---
name: core-web-vitals-triage
description: Rank Core Web Vitals failures by the traffic they actually cost. Use when CWV is failing or a speed audit is requested.
---

Pull CWV field data by URL group. Join each group to its GSC clicks over the last 28 days.
Ignore any failing group under 1% of total clicks — it is noise.
For each remaining group: metric failing | current value | threshold | clicks affected | the one technical cause.
Do not list generic advice like "optimise images" without naming the specific asset or script.
End with the single template to fix first.
