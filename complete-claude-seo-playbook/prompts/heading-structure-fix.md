# Fix the heading hierarchy of a page

**Area:** On-page optimization

**When.** Paste this with a page's headings when the outline was set by design choices rather than by structure.

## Prompt

```
Below is the heading list of one page in order, each line as heading level then heading text, plus the page's target keyword. If I have pasted only text with no levels, or no keyword, ask me for it before doing anything.

Audit the hierarchy. Check: exactly one H1 and it contains the target keyword or a clear synonym; no level is skipped (H2 to H4 with no H3 between); no heading is a styling choice (short bold labels like Note or Tip set as H3); headings are not questions where a plain statement is clearer, unless the section answers a People Also Ask question; every H2 states its subject so someone reading only headings understands the page; no two headings say the same thing.

Output a table, max 15 rows, one per problem, columns: current heading, level, problem, proposed heading, proposed level. Then the full corrected outline. Do not add sections the page does not have. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single heading change with the most effect, no alternatives.
```
