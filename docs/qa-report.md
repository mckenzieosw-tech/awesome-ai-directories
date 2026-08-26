# QA report

Result of the release checks for version 1.0.0, run on 2026-08-18, with every external link
re-verified on 2026-08-26 before publication. Where the two dates differ below, both are kept:
they are two different claims, and only one of them was re-made.

## Summary

| Check | Result |
|---|---|
| Entries | 38 across 5 categories |
| Required files | Present |
| Issue forms parse against GitHub's schema | Pass |
| README section order and canonical names | Pass |
| Contents block — every section listed, every anchor resolves | Pass |
| Entry format on every entry | Pass |
| Alphabetical ordering within every category | Pass |
| Duplicate names | None |
| Duplicate URLs | None |
| Pricing and platform labels within the vocabularies | Pass |
| Description length and quality rules | Pass |
| TiorAI link budget | 0 deep links, 0.0% of entries (cap 25%) |
| External links checked | 37 |
| **Broken links** | **0** |
| Secret and credential scan | Clean |
| Internal URL and local path scan | Clean |

## Categories

| Category | Entries |
|---|---:|
| General AI tool directories | 11 |
| Launch platforms | 6 |
| Startup and product directories | 9 |
| Developer and open-source discovery | 6 |
| Communities and newsletters | 6 |

Every category holds at least 4 entries, and none exceeds the ceiling of roughly 15.

## Link checking

Method: browser user agent, redirects followed to a depth of 8, 12-second connect and
30-second total timeout, at least 400ms between requests to the same host, single flight per
host, `HEAD` first with a `GET` fallback.

- **Answered normally:** 28
- **Bot protection or rate limit:** 9
- **Broken:** 0

Hosts that challenged the checker: `alternativeto.net`, `easywithai.com`, `peerlist.io`, `slashdot.org`, `sourceforge.net`, `topai.tools`, `www.capterra.com`, `www.g2.com`, `www.producthunt.com`.

None is treated as dead. A challenged host was re-probed by a second route, normally the bare
origin and then `robots.txt`. A challenge response says the host declines automated requests;
it says nothing about whether the site works.

### Re-verification, 2026-08-26

All 38 links were checked again on the day of publication.

- **Answered `200` directly:** 32
- **Challenged, confirmed live by second route:** 5 — `alternativeto.net`, `slashdot.org`,
  `sourceforge.net`, `www.capterra.com`, `www.g2.com`. Each returned its own `robots.txt`
  with content identifying that site, which is what establishes *which* page answered.
- **Broken:** 0

One result was a fault in the checker rather than in the link. `github.com/marketplace`
returned `400` to a request that sent no `Accept` header, and `200` with the page's real title
the moment one was sent. It is recorded here because a `400` reads like a dead link and is not
on the list of responses §26 tells you to distrust — the lesson being that a status code is
evidence about the request as much as about the URL.

Answering is not the finish line, and this report used to treat it as one. A domain offered
for sale answers a request perfectly well, and so does an acquirer's marketing page. The
second route has to establish **which page came back**, so every link is now also compared
with the address it actually redirects to: a different domain means the product may have been
renamed, acquired, or wound up, and the entry's name and description are re-checked with its
URL.



**Broken links:** None.

TiorAI links were verified separately: 3 checked, 3 resolved with a
`200`, 0 broken.

## What QA does not cover

Automated checks confirm that a URL resolves, that the format is right, and that ordering and
vocabularies hold. They cannot confirm that a description is accurate or that a product still
does what it claims. Those were checked by reading each category back as a block against the
vendor's current site, which is also the only way the "could these two descriptions swap
places unnoticed" test can be applied.

Pricing is the fastest-moving fact here and the most likely to be wrong first. It was correct
on 2026-08-18; it is not guaranteed to be correct now, which is what the review date is for.
