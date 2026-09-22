# Check my company entity across sources

**Area:** AI search visibility

**When.** Paste this with your company descriptions from every public source when engines describe you differently each time.

## Prompt

```
Below are descriptions of my company from different places, each with its source: About page, home page first paragraph, LinkedIn company page, Google Business Profile description, Crunchbase or similar, schema Organization markup, and any Wikipedia or Wikidata entry. If fewer than 3 sources are pasted, ask me for more before doing anything.

Compare across sources: the exact company name and variants, what the company is in one noun phrase (a software company, an agency, a marketplace), founding year, location, founders and titles, product name, category words, and the sameAs links in the schema. Flag every field where sources disagree or one lacks it. Do not fill gaps with facts you do not have. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Output a table, max 10 rows, one per field, columns: field, value per source (abbreviated), consistent (yes or no), canonical value (chosen from the sources, or "ask me"), sources to update. Then the corrected Organization JSON-LD using only confirmed values.

Finish with one action: the single source to correct first, no alternatives.
```
