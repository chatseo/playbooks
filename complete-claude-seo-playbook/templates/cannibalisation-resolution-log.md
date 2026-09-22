# Cannibalisation resolution log: [site]

**Export used:** [Search Console performance export, date range]
**Rule for a case:** two URLs each with more than [N] impressions on the same query over [days] days.

## Open cases

| Query | URL A | URL B | Decision | Status |
|---|---|---|---|---|
| [query] | [URL, position 28-day avg, clicks] | [URL, position 28-day avg, clicks] | [keep A / keep B / merge into A / differentiate] | [open / shipped / verified] |
| [query] | [URL, position, clicks] | [URL, position, clicks] | [decision] | [status] |
| [query] | [URL, position, clicks] | [URL, position, clicks] | [decision] | [status] |

## Decision rules

- **Keep one:** the loser gets a 301 to the winner, or its section is folded into the winner and the loser is redirected.
- **Differentiate:** rewrite title, H1 and intro of the weaker page around a different intent, and change internal anchors that point to it with the shared query.
- **Merge:** copy the unique sections of B into A, redirect B, update every internal link to B.

## Fix record

| Query | What shipped | Date shipped | Recheck date | Result after 28 days |
|---|---|---|---|---|
| [query] | [redirect / rewrite / merge, one line] | [date] | [date + 28 days] | [single URL now ranking? position before and after] |

## Fill-in notes

- Position is the 28-day average from the export, never a single-day number.
- A case is closed only when one URL holds the query for 28 days after the ship date.
- If Claude fills this, it uses only rows present in the export and writes "cannot compute from this data" where a page has no impressions on the query.
