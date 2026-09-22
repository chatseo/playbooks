# Rank the competitor keyword gap by topic

**Area:** Keyword research and clustering

**When.** Paste this with a content gap export when you want to know which competitor topics are worth chasing and which are noise.

## Prompt

```
Below is a keyword gap export (Ahrefs Content Gap or Semrush Keyword Gap) listing keywords where at least one competitor ranks and I do not, with columns keyword, volume, difficulty, and each competitor's position. If it is missing, ask me for it before doing anything.

Keep only keywords where at least two competitors rank in the top 10, volume is at least 50, and the keyword is not a competitor brand or product name. Group what remains by topic. For each group say whether I already have a page that could rank; ask for my page list if I have not pasted one. Score each group by competitors covering it, summed volume and median difficulty.

Output a table, max 20 rows, one per topic, sorted by summed volume descending, columns: topic, example keyword, keyword count, summed volume, median difficulty, competitors in top 10, my existing page or "none". If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the one topic to create or expand a page for first, no alternatives.
```
