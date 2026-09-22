# Triage Core Web Vitals by traffic cost

**Area:** Technical SEO and site audits · **Time:** 1 h · **Skill:** `core-web-vitals-triage`

**Goal.** Rank Core Web Vitals failures by the clicks on the pages they affect so the developer fixes the expensive ones first.

**When.** The Core Web Vitals report in Search Console shows poor URLs and the developer asks which to fix first.

## You need

- the Core Web Vitals report export from Search Console, mobile, with the URL groups and their failing metric
- a 28-day Search Console Pages export with clicks per URL
- PageSpeed Insights field data for one example URL per group, pasted as text

## Steps

1. Export the poor and needs improvement URL groups from the Core Web Vitals report and note the failing metric per group, LCP, INP or CLS.
2. Join each group's example URLs to the Pages export on URL and sum clicks per group, so each failing group carries the traffic it touches.
3. Paste the groups with clicks and the PageSpeed field data into Claude and ask it to rank the groups by clicks affected and name the likely cause per metric from the data shown.
4. Claude returns the ranked list with one fix per group, and writes cannot compute from this data where the field data is missing rather than guessing a cause.
5. Hand the developer the top three groups as three tickets, each with the URLs, the failing metric and the one fix, and re-export the report after 28 days.

**Done when the three highest-traffic failing groups are ticketed with a named metric and one fix each.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
