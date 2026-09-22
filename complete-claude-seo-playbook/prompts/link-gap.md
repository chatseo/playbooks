# Find domains linking to competitors, not me

**Area:** Link building and digital PR

**When.** Paste this with referring domain exports for you and your competitors when you want a prospect list that already links to your kind of site.

## Prompt

```
Below is a referring domains export for my site and for 2 to 4 competitors (Ahrefs Link Intersect, Semrush Backlink Gap, or one export per site), with columns domain, authority score, the linking page where given, and which sites it links to. If the exports are missing or cover only my site, ask me for the competitor data before doing anything.

Find domains that link to at least 2 competitors and not to me. Exclude directories, forums, coupon sites, domains with authority under 20, and properties owned by a competitor. Classify each remaining domain by how it probably linked (editorial mention, resource list, guest post, tool roundup, partner page), read from the linking page URL when given. Rank by the number of competitors linked, then by authority.

Output a table, max 20 rows, columns: domain, authority, competitors linked (count and names), link type, linking page example, angle for me (max 8 words). If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single domain to contact first and with which angle, no alternatives.
```
