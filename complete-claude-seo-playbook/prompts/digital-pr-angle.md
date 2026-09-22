# Find a PR angle in my own data

**Area:** Link building and digital PR

**When.** Paste this with a dataset you own when you want a story journalists can cite instead of another survey nobody ran.

## Prompt

```
Below is a dataset I own (a CSV or table from my product, my customers, or my own research) and one line on who I want coverage from. If the dataset is missing, ask me to paste it before doing anything; do not propose angles from public statistics.

Find the story. Compute only what the columns allow: counts, shares, medians, rank orders, and changes between two periods if both are present. Do not extrapolate to a population the data does not cover. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate. An angle qualifies when it is surprising against what the target audience assumes, specific (one number, one comparison), and defensible from the rows.

Output a table, max 5 rows, columns: headline (max 12 words), the one number, how it was computed from the columns, who would cover it (publication type), the weakness a journalist would raise. Then a Methodology paragraph, max 80 words, stating sample size, period, and what was excluded.

Finish with one action: the single angle to pitch and to whom, no alternatives.
```
