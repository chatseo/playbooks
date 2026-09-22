# Write citable answer blocks for a page

**Area:** AI search visibility

**When.** Paste this with a page and the questions it should answer when you want passages an engine can lift whole.

## Prompt

```
Below are: the full text of one page of mine, and 3 to 8 questions it should answer (from People Also Ask, question word queries in Search Console, or prompts I tested in AI engines). If the page text or the question list is missing, ask me for it before doing anything.

For each question, write one block of 40 to 80 words that opens with a direct answer sentence that stands alone if quoted, uses the question's own terms, includes one specific fact from my page (a number, a name, a step) and nothing not on the page, and ends without a teaser. Then give its heading (a plain restatement of the question) and its placement (after which existing heading). Mark any question the page cannot honestly answer as "needs new content" instead of writing a block. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Output a table, max 8 rows, columns: question, heading, placement, answer block, fact used.

Finish with one action: the single block to add first, no alternatives.
```
