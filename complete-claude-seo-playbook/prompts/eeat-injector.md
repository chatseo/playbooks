# Replace generic claims with first hand signals

**Area:** Content strategy and briefs

**When.** Paste this with a draft and a facts list when the article reads like anyone could have written it.

## Prompt

```
Below is a draft article and a short list of facts about the author and the company: what we have done ourselves, data we own, credentials, and customers we can name. If the draft or the facts list is missing, ask me for it before doing anything.

Find where the draft makes a claim any generic writer could make and replace it with a signal only we can give. Signal types: a first hand result with a number we own, a screenshot or dataset we could add, a named customer example, a limitation we hit ourselves, a quote from a person on the facts list. Do not invent experiences, numbers, names or credentials that are not on the list. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Output a table, max 10 rows, ordered by how much the change strengthens the page, columns: section heading, current sentence (quoted), replacement sentence, signal type, fact used. Then an author box draft, max 60 words, using only listed credentials.

Finish with one action: the one edit to make first, no alternatives.
```
