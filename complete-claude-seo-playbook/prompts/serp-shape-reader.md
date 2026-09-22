# Read what format a SERP rewards

**Area:** Competitor and SERP analysis

**When.** Paste this with the top 10 results you copied for one keyword when you want to know what to build before writing.

## Prompt

```
Below is a SERP I copied for one keyword: for each top 10 result the URL, title and page type (article, product, category, tool, video, forum), plus the features present (People Also Ask, video, images, shopping, AI Overview, featured snippet, local pack) in order. If results or features are missing, ask me for them before doing anything.

Count page types and name the dominant format (the type holding 5 or more of the 10; if none, call the SERP mixed and give the top two). Note whether the top 3 share a format the rest do not; whether results are mostly big brands or small sites, which says whether a new page can enter; and which features sit above the first organic result.

Output fixed sections: Shape table (page type, count, positions held), Dominant format, Features above organic, What to build (one page type, one content form: long guide, short answer, list, comparison table, video or tool, and a length band if the pasted pages give it, else "cannot compute from this data"). Never estimate.

Finish with one action: the single page format to build, no alternatives.
```
