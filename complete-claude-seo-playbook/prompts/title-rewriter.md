# Rewrite titles for low CTR pages

**Area:** On-page optimization

**When.** Paste this when pages rank on page one but get fewer clicks than their position should earn.

## Prompt

```
Below is my Search Console Pages export for the last 28 days (page, clicks, impressions, CTR, position) with the current title tag as a column, plus my brand name. If either is missing, ask me to paste it before doing anything.

Find pages where CTR falls below these floors: position 1 to 3, 15 percent; 4 to 6, 6 percent; 7 to 10, 3 percent. Keep pages with at least 200 impressions and position 10 or better. Exclude pages whose top query is branded. Rank by impressions multiplied by the CTR gap.

For each, write one new title of 50 to 60 characters: lead with the query the page already ranks for, state the format (guide, template, checklist, comparison), drop the brand name except on the home page. No clickbait, no year unless updated yearly.

Output a table, max 10 rows, columns: page, impressions, position, current CTR, expected CTR, current title, new title, character count. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single title to change today, no alternatives.
```
