# Check name, address and phone across listings

**Area:** Local SEO

**When.** Paste this with your canonical NAP and the listings you found when citations disagree with each other.

## Prompt

```
Below is my canonical name, address and phone (NAP) exactly as it should appear, and a list of listings I found (directory, the name, address and phone shown, and the URL). If the canonical NAP or the listings list is missing, ask me for it before doing anything.

Check consistency field by field. Count a mismatch when: the business name differs beyond case (an added keyword, a dropped Ltd, an old name); the street address differs beyond formatting (Suite versus Ste is formatting; a different number or postcode is a mismatch); the phone number differs beyond formatting; the listing duplicates another listing of the same location. Rank listings: Google Business Profile, Apple Maps, Bing Places, Facebook, industry directories, then the rest.

Output a table, max 25 rows, sorted by importance then by mismatches, columns: directory, URL, name match, address match, phone match, duplicate (yes or no), what to change. Then totals: listings checked, consistent, mismatched, duplicates. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Finish with one action: the single listing to correct first, no alternatives.
```
