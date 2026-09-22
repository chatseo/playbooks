# Turn dead pages into link prospects

**Area:** Link building and digital PR

**When.** Paste this with a list of dead pages and their backlinks when you have a page that can replace what died.

## Prompt

```
Below is a list of dead pages (404s or expired domains) in my niche: for each, the URL, what it was about, and an export of pages still linking to it (referring page, domain authority, anchor). If the linking page export is missing, ask me for it before doing anything.

For each dead page, match it to my page on the same subject (ask for my page list if needed). Skip dead pages with no equivalent; do not propose new pages. Keep referring pages with authority 20 or more, drop link lists with more than 50 outbound links, and drop referring pages on the dead site's own domain. Rank by authority.

Output a table, max 20 rows, columns: referring page, authority, dead URL it links to, anchor used, my replacement page, fit (exact, close, weak). Then one draft email, max 90 words, for exact fit rows, naming the broken link and offering the replacement, no flattery. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the one referring page to email first, no alternatives.
```
