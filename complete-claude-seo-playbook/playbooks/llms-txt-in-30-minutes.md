# Generate an llms.txt

**Area:** AI search visibility · **Time:** 30 min · **Skill:** `llms-txt-builder`

**Goal.** Publish an llms.txt at the site root that gives an AI model a clean summary of the site and links to its most useful pages.

**When.** You want to offer a curated entry point to the site for AI crawlers, and none exists yet.

## You need

- your sitemap URL list or a crawl export with URL, title and meta description
- a one-paragraph description of the site and who it serves
- the 20 to 40 pages you consider the most useful and current, chosen by you

## Steps

1. From the crawl export, keep only the pages you chose, with their title and description, and group them by section: docs, guides, product, pricing, about.
2. Paste the grouped list and the site description into Claude and ask it to write the llms.txt in the standard format: an H1 with the site name, a blockquote summary, then an H2 per section with one link and one line per page.
3. Tell Claude to use only the titles and descriptions given, to write nothing about pages not in the list, and to keep every page line under 20 words.
4. Claude returns the file as Markdown, plus a list of any page whose description was empty and needs a line written by you.
5. Write the missing lines, upload the file to the site root as /llms.txt, open it in a browser to confirm it serves as plain text, and put a quarterly review in the calendar.

**Done when /llms.txt is live at the root, serves as plain text, and every listed page has a one-line description.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
