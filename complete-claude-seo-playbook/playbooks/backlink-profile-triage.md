# Decide whether a backlink profile needs action

**Area:** Link building and digital PR · **Time:** 30 min · **Skill:** `toxic-link-triage`

**Goal.** Look at a suspicious set of backlinks and decide, with evidence, whether to ignore them, monitor them or disavow.

**When.** A backlink report shows a burst of odd referring domains, or a client asks whether they need to disavow.

## You need

- a backlinks export with referring domain, linking page, anchor text, first seen date and domain rating
- a 6-month Search Console Performance export at the site level, weekly, so any ranking impact is visible
- a note of any manual action shown in Search Console, or none

## Steps

1. Sort the backlink export by first seen date and isolate the domains that appeared in the last 90 days, with their anchor text and linking page.
2. Paste that subset, the weekly clicks series and the manual action note into Claude and ask it to describe the pattern: anchors, language, page types, and whether clicks moved after the burst.
3. Ask Claude to give one verdict, ignore, monitor or disavow, and to reserve disavow for the case where a manual action exists or the anchors are clearly manipulative and clicks fell after them.
4. Claude returns the verdict with the three facts from the data that support it, and says cannot compute from this data if the clicks series is missing.
5. If the verdict is disavow, build the domain list from the flagged rows only and upload it; otherwise file the summary and re-check in 3 months.

**Done when a written verdict with supporting facts exists and, if disavow, the file has been uploaded.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
