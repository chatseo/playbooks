# Schema spec sheet: [page template, e.g. product page]

**Applies to URLs matching:** [pattern]
**Schema type:** [Article / Product / FAQPage / LocalBusiness / HowTo / Organization]
**Why this type:** [the visible page content it describes, one line]
**Reference:** [schema.org type URL] and [Google structured data doc URL for this type]

## Properties

| Property | Required by Google? | Source of value | Example |
|---|---|---|---|
| [name] | [yes / recommended] | [CMS field / hard-coded / computed] | [value] |
| [image] | [yes / recommended] | [CMS field] | [URL] |
| [datePublished] | [yes / recommended] | [CMS field] | [ISO date] |
| [author.name] | [yes / recommended] | [CMS field] | [name] |
| [property] | [yes / recommended] | [source] | [example] |

## Rules the developer follows

- Every value must also be visible on the page. If it is not on the page, it is not in the markup.
- Ratings, prices and stock come from the live field, never from a static default.
- One block per page. Nest [linked type, e.g. Organization] inside, do not repeat it.

## Test plan

| Check | Tool | Result | Date |
|---|---|---|---|
| Markup parses with no errors | [Rich Results Test or Schema Markup Validator] | [pass / errors listed] | [date] |
| Values match the rendered page | [manual, 3 sample URLs] | [pass / mismatch listed] | [date] |
| Search Console enhancement report shows the type | [Search Console, after crawl] | [count valid / invalid] | [date] |

## Sign-off

- **Spec approved by:** [name, date]
- **Shipped on:** [date]
- **Recheck enhancement report on:** [date + 14 days]

## Fill-in notes

- "Source of value" is the field that actually exists in the CMS. If the field does not exist, that is a build task, not a placeholder value.
