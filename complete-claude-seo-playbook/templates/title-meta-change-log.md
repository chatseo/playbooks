# Title and meta change log: [site]

**Metric source:** [Search Console page export, 28-day window]
**Rule:** one change per page per 28 days, or you cannot tell which edit moved CTR.

## Changes

| URL | Field | Before | After | Date shipped |
|---|---|---|---|---|
| [URL] | [title / meta] | [old text] | [new text] | [date] |
| [URL] | [title / meta] | [old text] | [new text] | [date] |
| [URL] | [title / meta] | [old text] | [new text] | [date] |

## Baseline and recheck

| URL | Clicks, 28 days before | CTR before | Position before | Recheck date |
|---|---|---|---|---|
| [URL] | [n] | [%] | [28-day avg] | [ship date + 28 days] |
| [URL] | [n] | [%] | [avg] | [date] |

| URL | Clicks, 28 days after | CTR after | Position after | Verdict |
|---|---|---|---|---|
| [URL] | [n] | [%] | [avg] | [keep / revert / inconclusive] |
| [URL] | [n] | [%] | [avg] | [verdict] |

## Why each change

- [URL]: [the query the new title targets, and what the old one was missing]
- [URL]: [reason]

## Fill-in notes

- Compare CTR only when position moved less than one place. Otherwise mark "inconclusive" and note the position change.
- Google rewrites titles. On the recheck, note whether the search result showed your text: [yes / no / not checked].
- If Claude fills the recheck rows, it uses the export you paste and writes "cannot compute from this data" for pages missing from it.
