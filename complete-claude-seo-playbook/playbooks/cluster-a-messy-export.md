# Cluster a messy keyword export into topics

**Area:** Keyword research and clustering · **Time:** 1 h · **Skill:** `cluster-builder`

**Goal.** Turn a raw export of thousands of keywords into clean topic clusters, each mapped to one page to build or improve.

**When.** You have a large keyword export from a tool or a Search Console dump and no structure over it.

## You need

- the keyword export as CSV with a keyword column and at least a volume column
- a list of your existing URLs with their primary topic, one per line

## Steps

1. Clean the export first: lowercase every keyword, remove exact duplicates, and drop rows with fewer than 10 monthly searches so the noise does not swamp the clusters.
2. Split the file into batches of about 500 rows, because one huge paste makes the grouping sloppy, and paste the first batch into Claude with your URL list.
3. Ask Claude to cluster keywords that would be served by the same page, name each cluster with its head term, and attach an existing URL where one fits or write new page where none does.
4. Claude returns a table: keyword, cluster name, cluster total volume as the sum of the given rows, and the URL or new page label, with no guessed numbers.
5. Repeat for each batch, then paste all cluster names back into Claude and ask it to merge clusters that are the same topic under different names.
6. Sort the merged clusters by total volume and pick the top ten that map to new page, which becomes your content backlog.

**Done when every keyword sits in exactly one named cluster and each cluster points to one existing or planned URL.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
