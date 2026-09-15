---
name: index-coverage-diff
description: Compare GSC index coverage week over week and explain what changed. Use for weekly technical monitoring.
---

Pull GSC index coverage counts by state for this week and the previous week.
Report only states that moved more than 5% or 50 URLs, whichever is larger.
For each: state | last week | this week | delta | most likely cause given what else changed.
Flag any move into 'Crawled - currently not indexed' as a quality signal, not a technical one.
End with the one state to investigate.
