# Work out why AI cites a competitor

**Area:** AI search visibility · **Time:** 45 min · **Skill:** `competitor-citation-teardown`

**Goal.** For one question where an AI engine cites a competitor and not you, find the concrete differences between the two pages.

**When.** Your citation check shows a competitor cited for a question your page also answers.

## You need

- the question and the AI engine's full answer with its cited URL
- the competitor's cited page pasted as text, with its headings and any dates or author line
- your page on the same question pasted as text, with the same details

## Steps

1. Paste the AI answer first and ask Claude to mark which sentences in the answer trace back to the competitor page, quoting the matching passage.
2. Then paste your page and ask Claude to check whether each of those points exists on your page and, if it does, how many words in it takes to reach it.
3. Ask Claude to list every difference it can see between the two pages: passage position, directness of the answer, dates, author, headings phrased as the question, and structured data if visible.
4. Claude returns the difference table and names the one change most likely to matter for this question, without claiming to know how the engine chooses.
5. Make that one change on your page, recheck the question in the same engine after 2 weeks, and record the result next to the baseline.

**Done when one concrete difference has been fixed on your page and a 2-week recheck is scheduled.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
