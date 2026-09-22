# Audit internal anchor text

**Area:** Internal linking

**When.** Paste this with an inlinks export when you suspect anchors are generic, over optimised or pointing the wrong way.

## Prompt

```
Below is an internal links export (Screaming Frog All Inlinks or similar) with columns Source, Destination, Anchor, and Link Position if available. If it is missing, ask me for it before doing anything.

Audit anchors on the most linked destinations. For each destination with at least 5 inlinks, count its anchors. Flag: generic anchors (click here, read more, here, this page, learn more) as a share of the page's inlinks; one exact keyword anchor on more than 60 percent of inlinks (over optimised); anchors describing a different topic from the destination's title; the same anchor pointing to two different destinations. If Link Position is present, keep body links only and skip navigation and footer.

Output a table, max 15 rows, sorted by inlinks descending, columns: destination, inlinks, generic share, top anchor and its share, distinct anchors, flags, proposed anchor variants (max 3, each 3 to 7 words). If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the one destination whose anchors to rewrite first, no alternatives.
```
