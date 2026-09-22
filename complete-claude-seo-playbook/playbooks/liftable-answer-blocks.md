# Write passages AI engines can lift

**Area:** AI search visibility · **Time:** 45 min · **Skill:** `answer-block-writer`

**Goal.** Add a short, direct, self-contained answer passage to each key page so an AI engine can quote it without rewriting it.

**When.** Your pages answer the question eventually, but bury it under an introduction and a story.

## You need

- the list of question and page pairs from your citation check where you are not cited
- each page's content pasted as text
- the facts and numbers you are willing to state as your answer

## Steps

1. For each pair, paste the page and the question into Claude and ask it to locate where the page first answers the question and how many words a reader passes before reaching it.
2. Ask Claude to write a 40 to 70 word passage that answers the question in the first sentence, uses only facts from the page or the ones you supplied, and names the subject rather than using it.
3. Claude returns the passage, an H2 phrased as the question to sit above it, and a note of any fact it needed but did not have, written as cannot compute from this data.
4. Place the H2 and the passage within the first screen of the page, above the story, and keep the rest of the page as it was.
5. Recheck the question in the engines after 3 weeks and record whether the passage is now quoted.

**Done when every page in the list has a question H2 and a direct answer passage in the first screen.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
