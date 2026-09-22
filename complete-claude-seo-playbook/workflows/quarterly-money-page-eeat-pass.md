# The quarterly money-page EEAT pass

**Area:** Content strategy and briefs · **Cadence:** quarterly · **Time:** 4 h

**Trigger.** Start of each quarter, on the 20 pages that drove the most conversions in GA4 last quarter.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Export from GA4 the landing pages with the most conversions last quarter. Keep the top 20 in a sheet with their URL and conversion count. | manual | A sheet of 20 money pages with conversion counts. |
| 2 | For each page, paste its text plus what you have: author, credentials, customer numbers, screenshots, dates. Ask for the missing signals and where to add them. | `eeat-injector` | Per page, a list of concrete additions with the exact paragraph to insert them in. |
| 3 | Paste the page's three most asked questions and ask for a short, quotable answer block for each that stands on its own. | `answer-block-writer` | Three self-contained answer passages per page. |
| 4 | Give it the page type and the added elements. Ask which schema type applies and for the JSON-LD, with only facts that appear on the page. | `schema-picker` | One schema type and a JSON-LD block per page. |
| 5 | Ship the additions and the JSON-LD in the CMS, validate the markup in Google's Rich Results Test, and log the date per page. | manual | 20 updated pages with a ship date each. |

**Result.** Your top converting pages carry visible experience signals, quotable answers and valid schema, logged with a ship date so next quarter's GA4 export can be compared.
