# Find what blocks important pages from indexing

**Area:** Technical SEO and site audits

**When.** Paste this with a crawl export and robots.txt when pages you care about are not showing up in the index.

## Prompt

```
Below are: my robots.txt, and a Screaming Frog internal HTML export with columns Address, Status Code, Indexability, Indexability Status, Meta Robots, Canonical Link Element, and Inlinks. If the export or the robots file is missing, ask me for it before doing anything.

Find what stops important pages from being indexed. Check, in this order: URLs blocked by a robots rule that also carry a noindex (Google cannot see the noindex); noindexed URLs with 5 or more inlinks; canonical conflicts (the canonical target is itself noindexed, redirected, non 200, or canonicalised elsewhere); indexable URLs with 0 inlinks; canonicals pointing elsewhere on pages that receive traffic, and ask for my Search Console pages if you need them. Ignore URLs with parameters unless they have inlinks.

Output a table, max 20 rows, ordered by inlinks descending, columns: URL, problem type, evidence (the exact directive or canonical target), inlinks, fix. Then a count per problem type. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single blocker to remove first, no alternatives.
```
