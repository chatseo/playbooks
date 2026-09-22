# Design a hub and spoke for one topic

**Area:** Internal linking

**When.** Paste this with the pages you have on one topic when they exist as a pile rather than a structure.

## Prompt

```
Below are my pages on one topic (URL, title, top Search Console query, impressions), plus the topic name. If it has under 4 pages or no impressions, ask me for a fuller list first.

Choose the hub: the page whose query is the broadest head term with the most impressions, or say a new hub is needed if none targets it. Every other page is a spoke. Rules: each spoke links up to the hub with an anchor containing the head term; the hub links down to every spoke, saying what each answers; spokes link sideways only to the 2 spokes closest in sequence; off topic pages are excluded and listed. Merge spokes whose queries one page could answer.

Output: a Hub line (URL or "new page needed", plus the head term), a table of max 15 spokes, columns: spoke URL, sub topic, anchor to hub, sideways links (max 2), merge into (or none), then an Excluded list. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single link to add first, no alternatives.
```
