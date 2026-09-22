# Build an H2 outline from the SERP

**Area:** Content strategy and briefs · **Time:** 30 min · **Skill:** `outline-from-serp`

**Goal.** Get an H2 outline that covers what ranks and adds at least two sections nobody in the top 10 has.

**When.** You have a keyword approved for a new page and need the outline before the brief or the draft.

## You need

- the keyword and the intent you believe it carries
- the H1, H2 and H3 headings of the top 10 results, captured with a crawler or copied by hand
- a list of related questions from the People Also Ask box

## Steps

1. Capture the headings of the top 10 results into one file, one result per block, and add the People Also Ask questions at the bottom.
2. Paste the file into Claude with the keyword and ask it to list the headings that appear in at least 4 of the 10 results, which becomes the must-cover set.
3. Ask Claude to propose two sections that appear in none of the 10 results but answer a People Also Ask question or a step the ranking pages skip.
4. Claude returns an ordered outline of H2s, each with a one-line note on why it is there, and the two gap sections marked as the information-gain sections.
5. Reorder the outline so the reader gets the answer within the first two H2s, then approve it or send it back with one change.

**Done when an ordered H2 outline is approved with the must-cover set present and two gap sections marked.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
