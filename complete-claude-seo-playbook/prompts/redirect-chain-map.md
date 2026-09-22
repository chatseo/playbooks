# Map and collapse redirect chains

**Area:** Technical SEO and site audits

**When.** Paste this with a redirect chains report after a migration or when old URLs hop several times before landing.

## Prompt

```
Below is a Screaming Frog redirect chains report (each row: a starting URL, every hop with its status code, the final URL). If it is missing, ask me for it before doing anything.

Map the chains. Flag: chains of 2 or more hops; loops; chains ending in a 4xx or 5xx; chains mixing 301 and 302; http to https and www hops done separately (fold into one). For each start URL, state the final destination and the one direct redirect that replaces the chain. If I also paste an inlinks export, count internal links pointing at the first hop; those should be updated to the final URL.

Output a table, max 20 rows, sorted by hop count descending then by inlinks, columns: start URL, hops, status codes in order, final URL, final status, fix (collapse to one 301, fix loop, fix broken target, update internal links). Then totals: chains found, loops, broken endings. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single chain to collapse first, no alternatives.
```
