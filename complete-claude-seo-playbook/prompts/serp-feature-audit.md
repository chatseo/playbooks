# Find SERP features I can win

**Area:** Competitor and SERP analysis

**When.** Paste this with the features you saw per keyword and your positions when you want the features within reach, not the whole list.

## Prompt

```
Below is, per target keyword, the SERP features I saw (featured snippet, People Also Ask, video, image pack, AI Overview, shopping, local pack, top stories), who holds each, and my Search Console position for that keyword. If features or positions are missing, ask me for them before doing anything.

Rules: a featured snippet is winnable when I rank in the top 5 and I can answer more directly than the holder; a People Also Ask question when a page of mine can carry a 40 to 60 word answer under a matching heading; a video slot only if I have a video, so ask; image and shopping packs need a product or original image; a local pack needs a Google Business Profile. Ignore features held by the brand the query names.

Output a table, max 15 rows, columns: keyword, my position, feature, holder, winnable (yes, no, needs asset), what to add (heading, answer block, table, image, video), page. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single feature to target first, no alternatives.
```
