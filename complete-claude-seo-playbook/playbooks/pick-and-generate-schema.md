# Pick and generate the right schema

**Area:** On-page optimization · **Time:** 30 min · **Skill:** `schema-picker`

**Goal.** Choose the one schema type a page genuinely qualifies for and get valid JSON-LD you can paste and test.

**When.** A page type has no structured data, or a rich result report in Search Console shows errors on it.

## You need

- the page URL and its full visible content pasted as text
- the facts the schema needs, such as author, date, price, rating count, or address, taken from the page itself

## Steps

1. Paste the page content into Claude and ask which schema types the page qualifies for based on what is visibly on the page, and which it does not, with the reason.
2. Choose the single type Claude ranks first and paste the required facts, telling Claude that any property with no fact provided must be omitted, not filled in.
3. Claude returns the JSON-LD block for that one type with only the provided properties, plus a list of the properties it left out for lack of data.
4. Paste the block into the Rich Results Test or the Schema Markup Validator and fix any error it reports by editing the facts, not by adding invented values.
5. Deploy the block in the page head, then request indexing for the URL in Search Console and check the rich result report after a week.

**Done when the JSON-LD passes validation with zero errors and is live on the page.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
