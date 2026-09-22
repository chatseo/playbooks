# Kill redirect chains and loops

**Area:** Technical SEO and site audits · **Time:** 45 min · **Skill:** `redirect-chain-map`

**Goal.** Find every redirect chain and loop on the site and replace each with a single hop to the final URL.

**When.** After a migration, a redesign or a URL change, or when a crawl shows redirect chains.

## You need

- the redirect chains report from your crawler (Screaming Frog exports one under Reports, Redirects) with each hop and its status code
- the internal links export showing which pages link to the first URL of each chain

## Steps

1. Export the redirect chains report and the loops report and keep the columns for the starting URL, the number of redirects, each hop and the final status code.
2. Paste the report into Claude with the internal links export and ask it to list every chain with its final destination and every loop with no destination.
3. Ask Claude to output the rewrite rules needed so every starting URL redirects straight to its final URL, and to list source pages whose links should point to the final URL directly.
4. Claude returns two lists: the redirect rules to change, one per starting URL, and the internal links to update, and marks loops as needing a human decision on the destination.
5. Apply the rules, fix the internal links, choose a destination for each loop, and recrawl to confirm no chain longer than one hop remains.

**Done when a fresh crawl reports zero redirect loops and every redirect resolves in one hop.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
