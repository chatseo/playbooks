# The monthly title and meta round

**Area:** On-page optimization · **Cadence:** monthly · **Time:** 60 min

**Trigger.** Day 1 of the month, using the previous 28 days of Search Console data.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Export Search Console pages for the last 28 days. Paste it and ask for the pages in the top 10 whose CTR sits below what their position should get. | `low-ctr-finder` | A table of 10 to 20 URLs with position, impressions, CTR and the expected CTR. |
| 2 | For each URL, paste the current title and the top 3 queries. Ask for two title options per page, under 60 characters, that keep the main query. | `title-rewriter` | Two title options per URL with the query kept. |
| 3 | Paste the same URLs with their current meta descriptions and the chosen title. Ask for one description per page under 155 characters. | `meta-description-batch` | One meta description per URL. |
| 4 | Pick one title per page, ship titles and descriptions in the CMS, and note the ship date next to each URL in the table. | manual | The table with the shipped title and a date column. |
| 5 | After 28 days, re-export the same report and compare CTR per URL. Revert any page whose CTR dropped. | manual | Per URL, CTR before and after and a keep or revert decision. |

**Result.** A monthly batch of 10 to 20 rewritten titles and descriptions with a dated table that shows which ones lifted CTR and which were reverted.
