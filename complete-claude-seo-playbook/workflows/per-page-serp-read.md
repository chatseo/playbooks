# The per-page SERP read before writing

**Area:** Competitor and SERP analysis · **Cadence:** per new page · **Time:** 25 min

**Trigger.** A target query is assigned to a new page and nobody has looked at its results page yet.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Give it the target query, the country and the top 10 URLs with their titles. Ask for the dominant intent and whether the SERP is mixed. | `intent-classifier` | One intent label and a mixed or clean verdict. |
| 2 | Paste the top 10 with their page type, word count if you have it, and first H2s. Ask what format and length rank and what angle they share. | `serp-shape-reader` | The ranking format, length range and shared angle. |
| 3 | List the features on the page: People Also Ask, videos, images, featured snippet, AI overview, shopping. Ask which ones your page can realistically own. | `serp-feature-audit` | Features to target and the element the page needs for each. |
| 4 | Paste the intent, shape and features into the brief and hand it to the content build. Reject the brief if the intent is transactional and the page is a guide. | manual | A brief with a SERP section, or a rejected assignment. |

**Result.** Every brief carries the intent, the format that ranks and the features to target before a word is written, and mismatched assignments die here rather than after publishing.
