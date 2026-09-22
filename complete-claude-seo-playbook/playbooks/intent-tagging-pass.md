# Classify a keyword list by intent

**Area:** Competitor and SERP analysis · **Time:** 30 min · **Skill:** `intent-classifier`

**Goal.** Tag every keyword in a list as informational, commercial, transactional or navigational so each one gets the right page type.

**When.** You have a keyword list ready and need intent before mapping keywords to pages.

## You need

- the keyword list as CSV with volume
- for the 30 highest-volume keywords, the titles of the top 5 results, captured by hand or with a SERP tool

## Steps

1. Paste the keyword list into Claude in batches of 300 and ask it to tag each keyword by intent from its wording alone, and to mark uncertain ones.
2. For the 30 highest-volume keywords and every uncertain one, paste the top 5 result titles and ask Claude to confirm or change the tag from what actually ranks.
3. Claude returns keyword, intent tag, confidence, and the page type that intent calls for: guide, comparison, category, product or brand page.
4. Spot-check 10 random tags against a live search yourself and, if more than two are wrong, rerun the batch with the corrected examples as guidance.
5. Save the tagged list and use the page type column as the input to your keyword-to-page mapping.

**Done when every keyword carries an intent tag and a page type, and a 10-keyword spot check passed.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
