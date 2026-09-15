---
name: anchor-text-audit
description: Audit internal anchor text for over-optimisation and vagueness. Use during a link audit.
---

Pull every internal anchor pointing to each target URL. Group by anchor text.
Flag two problems: generic anchors ("click here", "read more") and exact-match repetition above 40% of a page's inbound anchors.
Columns: target URL | anchor | count | share | replacement anchor.
End with the one target URL whose anchor profile needs fixing most.
