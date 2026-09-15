---
name: orphan-finder
description: Find pages with no internal links pointing to them. Use during a site audit.
---

Build the internal link graph from a crawl. Flag every indexable URL with zero inbound internal links.
Join each orphan to its GSC impressions — an orphan with impressions is a real loss, one with none may deserve to be cut.
Columns: orphan URL | impressions | topic | 3 existing pages that should link to it.
Cap at 20.
End with the one orphan to link first.
