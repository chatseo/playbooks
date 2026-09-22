# The entity and llms.txt setup

**Area:** AI search visibility · **Cadence:** once, then after any migration · **Time:** 2 h

**Trigger.** The first time you take AI answers seriously, then whenever the site structure or the company facts change.

## Steps

| # | Do | Uses | Hands over |
|---|---|---|---|
| 1 | Paste how your company, product and founders are described on the site, on your profile pages, on Wikipedia or Crunchbase if present, and in your schema. | `entity-consistency` | A list of conflicting names, descriptions and facts with the source of each. |
| 2 | Fix the conflicts at every source you control and note which external sources you cannot edit. | manual | A corrected set of descriptions and a list of external mismatches. |
| 3 | Give it the corrected company description and the 20 to 40 pages that best explain what you do. Ask for the llms.txt file with one line per page. | `llms-txt-builder` | An llms.txt file ready to upload. |
| 4 | Give it the corrected facts and ask for the Organization JSON-LD, using only what appears on the site. | `schema-picker` | An Organization JSON-LD block. |
| 5 | Upload llms.txt to the site root, add the JSON-LD to the homepage, and check both load in a browser. | manual | Both files live and verified. |

**Result.** One consistent description of who you are across everything you control, an llms.txt at the root and Organization schema on the homepage, redone only when the facts change.
