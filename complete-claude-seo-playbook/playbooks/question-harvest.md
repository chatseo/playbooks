# Harvest the real questions for a topic

**Area:** Keyword research and clustering · **Time:** 30 min · **Skill:** `question-harvester`

**Goal.** Collect the questions people actually ask about one topic, in their words, and pick the ones worth a section or a page.

**When.** You are planning a guide or an FAQ and do not want to invent the questions yourself.

## You need

- the topic and the audience in one sentence
- raw question sources: People Also Ask captures, a Search Console query export filtered to words like how, what, why, can, and the question tab of a keyword tool
- optionally, 20 to 50 support tickets, forum threads or sales call notes on the topic

## Steps

1. Gather every question source into one text file, one question per line, keeping the original wording even when it is clumsy, and note the source next to each.
2. Paste the file into Claude with the topic sentence and ask it to merge duplicates that mean the same thing, keeping the most common phrasing as the label.
3. Ask Claude to tag each merged question as answerable in two sentences, needs its own section, or needs its own page, based only on the question itself.
4. Claude returns a table: question, source count, tag, and the questions it merged under it, without adding questions that were not in the file.
5. Take every question tagged needs its own section and slot it into your outline, and add the needs its own page ones to the content backlog.

**Done when your outline holds the section questions in the searcher's words and the page-level questions are in the backlog.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
