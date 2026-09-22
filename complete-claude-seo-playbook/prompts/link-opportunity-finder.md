# Find internal links to a money page

**Area:** Internal linking

**When.** Paste this when one page needs to rank and you want the exact pages, anchors and sentences to link from.

## Prompt

```
Below are: the URL and target keyword of one money page, and a list of my other pages with URL, title, top 3 Search Console queries and impressions. If the money page or the page list is missing, ask me for it before doing anything.

Find internal link opportunities. A candidate qualifies when its title or queries share the money page's topic and it does not already link there. Ask for the money page's inlinks; if I cannot give them, mark that column unknown. Prefer candidates with more impressions; they are crawled and read more. For each candidate write the anchor (3 to 7 words, containing the target keyword or a close variant, no two identical) and the body sentence it should live in, never footer or sidebar.

Output a table, max 10 rows, ordered by impressions descending, columns: candidate URL, shared topic, impressions, already links (yes, no, unknown), anchor, sentence. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single link to add first, no alternatives.
```
