# Write responses to a batch of reviews

**Area:** Local SEO

**When.** Paste this with unanswered reviews when you want replies that are specific, calm and not a keyword dump.

## Prompt

```
Below are reviews from my Google Business Profile (stars, text, reviewer first name, date), plus one line on my business and how I sign responses. If either is missing, ask me for it before doing anything.

Write one response per review, max 70 words each. For 4 and 5 stars: thank by first name, echo one specific thing they mentioned, name the service in plain words once, invite them back with something concrete. For 3 stars: thank, acknowledge the specific shortfall, say what changes. For 1 and 2 stars: no defensiveness, acknowledge the specific issue, take it offline with a named person and a channel, never argue facts or disclose customer details. Flag any review that reads as fake or off topic for reporting instead of answering. Never offer discounts in public. Do not invent details about the visit. If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Output a table, max 20 rows, columns: reviewer, stars, response, flag (respond, report, escalate).

Finish with one action: the single review to answer first, no alternatives.
```
