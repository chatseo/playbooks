---
name: redirect-chain-map
description: Find redirect chains and loops wasting crawl budget and link equity. Use during a migration or technical audit.
---

Crawl the URL list and follow every 3xx to its final destination.
Report only chains of 2+ hops, and any loop.
Columns: start URL | hops | final status | inbound internal links | inbound external links.
Sort by external links, because that is where equity is leaking.
End with the one chain to flatten first.
