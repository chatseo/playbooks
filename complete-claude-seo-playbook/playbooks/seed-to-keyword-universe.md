# Build a keyword universe from one seed

**Area:** Keyword research and clustering · **Time:** 45 min · **Skill:** `seed-expander`

**Goal.** Turn a single seed keyword into a scored list of a few hundred related terms you can actually plan content against.

**When.** You are opening a new topic and have one seed keyword and no list yet.

## You need

- one seed keyword and a one-line description of the site it is for
- a keyword tool export for that seed (Ahrefs, Semrush or Keyword Planner) with volume and difficulty columns
- the list of URLs you already have on the topic, if any

## Steps

1. Export every keyword idea your tool gives for the seed, including matching terms and questions, keeping the volume and difficulty columns, and save it as a CSV.
2. Delete rows with zero volume and any brand names that are not yours, then paste the remaining rows into Claude with the site description and the seed.
3. Ask Claude to group the terms by the job the searcher is doing, flag terms that do not belong to the topic, and mark any volume it was not given as cannot compute from this data.
4. Claude returns a table with one row per term, the group it belongs to, a keep or drop flag, and the difficulty as given, never estimated.
5. Pick the three groups with the best volume-to-difficulty ratio for your site and mark each as a future cluster, dropping the rest for now.

**Done when you have a CSV of kept terms grouped into named clusters and three clusters chosen for the next content plan.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
