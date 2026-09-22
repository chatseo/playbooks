# Write meta descriptions in batch

**Area:** On-page optimization

**When.** Paste this with a list of URLs when descriptions are blank, duplicated or written years ago.

## Prompt

```
Below is a list of up to 20 URLs, each with its H1, its current meta description (blank if none) and its top Search Console query. If either is missing, ask me for it before doing anything.

Write one meta description per URL, 120 to 155 characters, that starts with the outcome the reader gets, contains the top query in natural wording within the first 100 characters, matches the page type (a product page says what it is and for whom, a guide what it teaches, a comparison what is compared), and ends with a concrete reason to click, not "learn more". Do not repeat the H1 verbatim. Do not claim numbers, prices or awards absent from the input. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Flag URLs whose current description is blank, duplicated, or under 70 characters, and put those first.

Output a table, max 20 rows, columns: URL, flag reason, new description, character count, top query included (yes or no).

Finish with one action: the one URL to update first, no alternatives.
```
