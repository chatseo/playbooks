# Turn a cluster into a hub and spokes

**Area:** Internal linking · **Time:** 1 h · **Skill:** `hub-spoke-builder`

**Goal.** Take one topic cluster and define the hub page, the spoke pages and the exact links between them so the cluster reads as one structure.

**When.** You have several pages on one topic that do not link to each other and no page acts as the entry point.

## You need

- the cluster's keyword list with the URL currently ranking for each, from your clustering or Search Console
- the current internal links between those URLs, from the crawl inlinks export

## Steps

1. List every URL in the cluster with its main query and volume, and mark which pages currently link to which, from the inlinks export.
2. Paste the list into Claude and ask it to name the hub as the page serving the broadest query, and each spoke as a page serving one narrower query.
3. Ask Claude to output the full link map: hub links to every spoke with a descriptive anchor, every spoke links back to the hub, and spokes link sideways only where the topics touch.
4. Claude returns a table of source, destination and anchor for every link to add, and a list of pages that do not fit the cluster and should be left out.
5. Add the links in the CMS, hub first, and add a short section on the hub that introduces each spoke so the links sit in real text.

**Done when the hub links to every spoke, every spoke links to the hub, and the link map has been applied in full.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
