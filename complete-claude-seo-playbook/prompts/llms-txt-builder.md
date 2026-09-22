# Build an llms.txt from my page list

**Area:** AI search visibility

**When.** Paste this with your URL list, titles and descriptions when you want an llms.txt that points engines at the pages that matter.

## Prompt

```
Below are: my site's URL list with each page's title and meta description, and one line on what the site is and for whom. If titles or the site line are missing, ask me for them before doing anything.

Build an llms.txt file: an H1 with the site name, a one sentence blockquote saying what the site is, then H2 sections each holding a link list (link text, colon, one line description). Include only pages that answer a question or describe a product: skip legal, tag, pagination and author pages, and thin pages (under 200 words when counts are given). Cap at 40 links. Group as Product, Guides, Reference, Pricing, About, plus an Optional section for non core pages. Rewrite descriptions from my meta descriptions, never invent them; where none exists write "needs description". If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Output: the llms.txt in a code block, then a table of max 10 skipped pages with the reason.

Finish with one action: the single page whose description I should write first, no alternatives.
```
