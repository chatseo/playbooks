# Pick schema types and draft JSON-LD

**Area:** On-page optimization

**When.** Paste this with a page's visible text when you want structured data that the page can honestly carry.

## Prompt

```
Below are: the URL and full visible text of one page, and its page type if I know it (article, product, FAQ, how to, local business, software). If the text is missing, ask me to paste it before doing anything.

Pick the schema types this page can honestly carry and draft the JSON-LD. Rules: choose only types whose required properties are visible on the page (a FAQPage needs visible question and answer pairs, a Product with offers needs a visible price, a HowTo needs numbered steps). Do not add ratings, review counts, prices, dates or author names that are not in the text. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate. Prefer one main type plus at most two supporting types.

Output: a table with max 3 rows, columns: schema type, why it fits, required properties found, properties missing; then one JSON-LD block using a single @graph; then a list of max 5 things to verify before deploying.

Finish with one action: the single property I must confirm on the page before adding this markup, no alternatives.
```
