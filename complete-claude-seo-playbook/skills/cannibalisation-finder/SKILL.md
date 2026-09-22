---
name: cannibalisation-finder
description: Find pages competing against each other for the same query. Use when rankings fluctuate or traffic is flat.
---

Pull GSC query-page pairs for the last 90 days. Flag any query where 2+ URLs each took impressions.
Only report cases where the alternate URL took over 10% of impressions — below that it is noise.
Columns: query | URLs | impressions split | clicks | which URL should win and why.
Recommend one of: merge, differentiate intent, or canonicalise. Never all three.
End with the one query costing the most clicks.
