# Cluster a keyword export into pages

**Area:** Keyword research and clustering

**When.** Paste this with a raw keyword export when you need to turn hundreds of keywords into a short list of pages.

## Prompt

```
Below is my keyword export (Ahrefs or Semrush) with columns keyword, volume, difficulty, and the URL currently ranking for me if any. If the export is not pasted below, ask me for it before doing anything.

Cluster the keywords so that one page can rank for every keyword in a cluster. Two keywords belong together when a searcher would be satisfied by the same page: same intent, same entity, same format. Treat modifiers like best, vs, pricing and how to as different intents and keep them in separate clusters even when the head term matches. Move keywords with volume under 10 to an ignored list. Rank clusters by summed volume, then by the lowest median difficulty.

Output a table, max 25 clusters, columns: cluster name, primary keyword, keyword count, summed volume, median difficulty, current ranking URL if one exists, page type (guide, comparison, product, tool). Below it, give the ignored keywords as a count only. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the one cluster to build or optimise first, no alternatives.
```
