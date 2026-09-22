# Redirect map: [migration or change name]

**Go-live date:** [date]  **Old host:** [domain]  **New host:** [domain]
**Source of old URL list:** [crawl + Search Console pages export + backlinked URLs, date]
**Total old URLs:** [n]  **Mapped:** [n]  **Unmapped:** [n]

## Map

| Old URL | New URL | Type | Rule | Status |
|---|---|---|---|---|
| [old URL] | [new URL] | [301] | [one-to-one / pattern] | [pending / live / verified] |
| [old URL] | [new URL] | [301] | [rule] | [status] |
| [old URL] | [new URL] | [301] | [rule] | [status] |

## Pattern rules

| Pattern (old) | Pattern (new) | URLs covered | Tested on |
|---|---|---|---|
| [/blog/(.*)] | [/articles/$1] | [n] | [3 sample URLs] |

## URLs with no equivalent

| Old URL | Backlinks | Clicks, last 90 days | Decision |
|---|---|---|---|
| [URL] | [n referring domains] | [n] | [redirect to closest parent / 410 / keep live] |

## Must-not-break list

- [URL with the most referring domains]
- [URL with the most clicks]
- [URLs that appear in ads, emails or print]

## Verification after go-live

| Check | Result | Date |
|---|---|---|
| Every old URL returns a single 301 (no chains, no 302) | [pass / list failures] | [date] |
| Old sitemap removed, new sitemap submitted | [done / not done] | [date] |
| Search Console Change of address filed (domain moves only) | [done / not applicable] | [date] |
| Top 50 old URLs by clicks spot-checked in a browser | [pass / failures] | [date] |

## Rules

- Redirect to the page that answers the same intent, not to the home page.
- No redirect points at a URL that itself redirects.
