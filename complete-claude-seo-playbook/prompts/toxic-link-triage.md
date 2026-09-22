# Triage a backlink profile for toxic links

**Area:** Link building and digital PR

**When.** Paste this with a backlinks export when a spike of strange links appeared and you want to know whether to act or ignore.

## Prompt

```
Below is a backlinks export (Ahrefs, Semrush or Search Console Links) with columns referring page, domain, authority, anchor, first seen, and dofollow or nofollow if present. If it is missing, ask me for it before doing anything.

Triage without over disavowing. Bucket every domain as harmless (nofollow, or authority under 10 with a generic anchor), watch (exact match money anchors from unrelated sites, or 20 or more links from one domain in a short window), or act (link farms, hacked pages, foreign language spam with commercial anchors, paid network patterns like one template across many domains). Volume alone is not toxic. Flag a spike when over 30 percent of first seen dates fall inside 30 days.

Output a table, max 20 rows, watch and act only, act first then by authority, columns: domain, links, authority, anchor sample, first seen, bucket, reason. Then totals per bucket and a domain: format disavow list for the act bucket only. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single step to take with the act bucket, no alternatives.
```
