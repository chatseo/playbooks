# Separate real decay from noise

**Area:** Google Search Console analysis

**When.** Paste this with a period comparison export when traffic is down and you need to know which pages actually decayed.

## Prompt

```
Below is my Search Console Pages export comparing the last 3 months with the previous 3 months (page, clicks, impressions and position for both periods). If I pasted a single period, ask me for the comparison export before doing anything.

Detect decay, not noise. A page decays when clicks fell by 20 percent or more and by at least 30 clicks, and position worsened by 1 or more. Separate from that: pages where clicks fell but position held (demand fell or a SERP feature appeared), and pages where position held, impressions rose and CTR fell (something pushed us down visually). Ignore pages under 100 clicks in the earlier period. Rank by clicks lost.

Output a table, max 15 rows, columns: page, clicks before, clicks after, change in percent, position before, position after, pattern (decay, demand drop, visual push), first check (refresh, SERP, indexing). Then total clicks lost across decaying pages. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single page to open first and what to check, no alternatives.
```
