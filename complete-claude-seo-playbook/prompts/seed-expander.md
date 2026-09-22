# Expand seed keywords into candidates

**Area:** Keyword research and clustering

**When.** Paste this when you have a handful of seed terms and need a wider candidate list before opening a keyword tool.

## Prompt

```
You are helping me expand a seed keyword list before I run it through a keyword tool. Below are my 3 to 10 seed keywords, one line describing what the site sells, and one line on who buys it. If any of the three is missing, ask me for it before doing anything.

For each seed, generate candidates in four buckets: modifiers (best, vs, alternative, pricing, template, example), questions (how, why, what, can), audience (for small business, for agencies, for beginners), and job to be done (the verb a buyer would type). Skip any candidate that is only a plural or a word order swap of another. Skip candidates that describe a different product category than the one I described.

Output one table, max 40 rows, columns: candidate, seed, bucket, likely intent (informational, commercial, transactional), why a buyer types it (max 10 words). Do not write search volumes or difficulty scores. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single bucket I should paste into my keyword tool first and why, no alternatives.
```
