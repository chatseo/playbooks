# Surface pages buried too deep

**Area:** Internal linking

**When.** Paste this with a crawl export when important pages sit four or more clicks from the home page.

## Prompt

```
Below is a Screaming Frog crawl export (Address, Crawl Depth, Inlinks, Indexability) and, if I have it, a Search Console Pages export with clicks and impressions. If the crawl is missing, ask me for it before doing anything.

Too deep means crawl depth 4 or more (home page is 0). Rank by impressions if given, otherwise by inlinks. Ignore paginated URLs, parameters and legal pages. For each, propose the shallowest existing page that could link to it (a category, a hub, a depth 1 to 2 page on the same topic); the new depth is that page's depth plus 1. If over 30 percent of indexable URLs sit at depth 4 or more, say so and name the structural cause (pagination only, missing category links, no related links).

Output a table, max 20 rows, columns: URL, current depth, inlinks, impressions, proposed linking page, new depth. Then a depth distribution table (depth, URL count). If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single page to surface first and from where, no alternatives.
```
