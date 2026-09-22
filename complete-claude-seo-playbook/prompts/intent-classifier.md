# Classify keyword intent from the query

**Area:** Competitor and SERP analysis

**When.** Paste this with a keyword list when you need intent labels before deciding what page type each one gets.

## Prompt

```
Below is a list of keywords, one per line, with volume if I have it. If the list is missing, ask me to paste it before doing anything.

Classify each keyword's dominant intent using only the words in the query: informational (how, what, why, guide, examples), commercial investigation (best, top, vs, review, alternative, comparison), transactional (buy, pricing, download, sign up, near me, a product plus discount), navigational (a brand or site name). When a query could carry two intents, give the primary and secondary and say what would settle it (the SERP format, which I can paste). Mark queries that are a competitor's brand. For each intent, name the page type that usually satisfies it (guide, comparison, product page, category, tool, home page).

Output a table, max 50 rows, columns: keyword, volume, primary intent, secondary intent (or none), confidence (high, medium, low), page type, note. Then a count per primary intent. Do not invent volumes. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the one intent group to build pages for first, no alternatives.
```
