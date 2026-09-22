# Check my page against the SERP intent

**Area:** Competitor and SERP analysis

**When.** Paste this when a page ranks badly for its keyword and you suspect the page type is the problem, not the content.

## Prompt

```
Below are: my page's URL and main headings, its target keyword, and the titles and page types of the top 10 results for that keyword. If my page or the SERP is missing, ask me for it before doing anything.

Compare what my page is (type, promise, first 100 words) with what the SERP rewards (the type held by 5 or more results). Mismatch cases: a product page against a SERP of guides; a broad guide against comparisons; a page answering a different question than the query; a locale the SERP does not show. Decide one of: keep, retarget (change the keyword), rebuild (change the page type), split (a second page for the other intent). Do not recommend rebuild when a retarget keeps current traffic; ask for the page's Search Console queries if needed.

Output fixed sections: My page type, SERP type and count, Mismatch (yes or no, evidence quoted), Decision, Reason (max 3 lines). If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single change the decision implies, no alternatives.
```
