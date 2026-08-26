# Candidate pool

What was considered for this list, what was verified, and what was left out.

Two things are deliberately absent, and neither is an oversight:

- **Internal scores and per-product rejection notes.** Editorial scoring stays out of a
  public repository. Exclusions below are given as neutral categories, not as judgements
  about named companies.
- **A per-candidate TiorAI URL map.** Capturing a TiorAI link for every candidate would
  produce exactly the backlink list this portfolio's own rules prohibit.

## Sources of candidates

| Source | Role |
|---|---|
| TiorAI's published AI tools catalogue | Read-only, used to shortlist candidates and to confirm product identity. No description or stored URL was carried through |
| Direct knowledge of the category | Used to fill gaps the catalogue does not cover well and to remove products that have since shut down or been absorbed |
| The vendor's own site | The authority for every fact that ships: current name, canonical URL, pricing tier, platform support |

Category assignment, pricing, and platform labels from the catalogue were treated as
*signals*, never as published values. The catalogue's own taxonomy is far too large and too
redundant to publish, so this repository defines its own.

## Pool

| Stage | Count |
|---|---:|
| Candidates considered | 114 |
| Shortlisted after scope filtering | 53 |
| **Published** | **38** |

## Why candidates were dropped

- **Link farm.** By a wide margin the largest exclusion. A great many "AI directories" exist to sell a dofollow link and have no readership at all.
- **Scraped catalogue.** Sites whose entire listing set was lifted from two or three larger directories, often including the same descriptions and the same dead entries.
- **No submission route.** A directory nobody can get into is not useful to this audience, however good its editorial is.
- **Dead or abandoned.** Openbase, a package review directory, closed in 2023 and was shortlisted before verification caught it. Several directories that were prominent two years ago have added nothing since. Where the most recent listing is more than a year old, the site was dropped.
- **Paid placement presented as editorial.** Directories where the ranking is the pricing table, without saying so.
- **Submission terms unknowable.** A small number of otherwise credible sites were dropped because their terms could not be established at all, and a table row of two `Unknown` values helps nobody.

## Verification

Every published entry had its official URL resolved over HTTP before release, following
redirects to the canonical destination. 37 distinct external URLs were checked:
28 answered normally, 9 returned a bot-protection or rate-limit
response, and 0 were broken.

A `401`, `403`, `405`, `429`, or `999` was never treated as evidence that a site is dead. Each
was re-probed by a second route and reasoned about rather than acted on automatically. No
entry was removed on the basis of a single failed request.

Time-sensitive facts — pricing tier, whether a free plan still exists, product availability,
renames, acquisitions, shutdowns, platform support — were re-checked against the vendor at
build time regardless of what the catalogue record said.
