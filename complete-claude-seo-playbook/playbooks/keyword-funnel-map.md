# Map keywords to funnel stage

**Area:** Competitor and SERP analysis · **Time:** 30 min · **Skill:** `buying-stage-mapper`

**Goal.** Assign every keyword in a cluster to awareness, consideration or decision so the content plan covers the whole path to purchase.

**When.** Your content is all top-of-funnel guides and nobody can say which keywords bring buyers.

## You need

- the keyword list with volume and, if you have it, the URL currently ranking
- a one-paragraph description of the product, who buys it, and what they compare it with before buying

## Steps

1. Paste the keyword list and the product description into Claude and ask it to tag each keyword as awareness, consideration or decision, with the wording cue it used.
2. Ask Claude to total the volume per stage from the given numbers and to list the decision-stage keywords with no ranking URL, which are your uncovered buying queries.
3. Claude returns the tagged list, the volume per stage, and the uncovered decision keywords, without adding keywords that were not in the list.
4. If the decision stage has fewer than 10 keywords with a ranking URL, make the uncovered decision keywords the next five pages to build, in volume order.
5. Save the stage column into your keyword map so every future brief states the stage it serves.

**Done when every keyword has a stage and the uncovered decision keywords are at the top of the content backlog.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
