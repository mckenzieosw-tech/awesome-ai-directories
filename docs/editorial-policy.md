# Editorial policy

The rules this repository is built and maintained by. The README's
"How directories are selected" section is the short version; this is the full one.

## Scope

Directories, discovery platforms, and launch sites where someone who has built an AI product can get it listed. The audience is the person doing the submitting, not the person browsing.

That framing decides the columns. A reader here already knows what a directory is; what they cannot easily find out is whether submission is open or curated, and whether it costs anything. Those two facts are scattered across submission pages, pricing tables, and support articles, and they are the reason this repository exists as a table rather than a list.

TiorAI runs one of the directories listed. It appears once, in its alphabetical position, with the same two columns filled in by the same rules as everything else.

## What qualifies

- It lists products other people made, and accepts submissions or nominations.
- It is currently maintained, with listings added within the past few months.
- Its submission terms are discoverable without an account or a sales conversation.
- There is enough public information to describe it accurately.
- It covers something the entries already in that category do not.

## What does not

- Link farms and directories that exist only to sell backlinks.
- Sites whose entire catalogue is scraped from other directories.
- Directories with no submission route at all.
- Paid-only placements dressed up as editorial selection.
- Broken, parked, or login-walled sites with no public information.
- Products that have shut down or been folded into something else.
- Affiliate landing pages, coupon sites, and lead-capture funnels.
- Near-identical clones with no meaningful difference from something already listed.
- Anything whose main activity is clearly illegal, and NSFW-focused products.
- Anything submitted purely as a promotional exercise.

## Descriptions

One sentence, 8 to 25 words, 35 at the absolute maximum, ending in a full stop. Written for
this repository rather than adapted from a vendor's homepage, and rewritten if a neighbouring
entry could swap places with it unnoticed.

Banned outright: superlatives (*best*, *leading*, *revolutionary*, *cutting-edge*,
*game-changing*, *world-class*, *ultimate*, *powerful*, *seamless*, *unleash*), `AI-powered`
as an opening, unverifiable claims about users, funding, or awards, and the em dash inside a
description, which is reserved as the entry separator so the format stays machine-parseable.

## Metadata vocabularies

Closed sets. A term outside them is a defect, not a judgement call. Exactly one value per
cell — these are columns, not labels, so a row that cannot choose uses `Unknown` rather than
two values or an empty cell.

**Submission** — how a product gets listed:
`Open` · `Curated` · `Invite` · `Unknown`

`Open` means anyone can submit and the listing appears, subject to basic checks. `Curated`
means submissions are reviewed and can be declined on editorial grounds. `Invite` means the
operator chooses the listings and there is no public submission route.

**Pricing** — what submission costs:
`Free` · `Paid` · `Free/Paid` · `Unknown`

`Free` means a free submission route exists and is the normal path. `Paid` means submission
requires payment. `Free/Paid` means a free route exists alongside a paid one that skips the
queue or adds placement.

This is deliberately **not** the portfolio's tool-pricing vocabulary. That set answers "what
does this product cost to use", and every directory here is free to read; the question a
submitter actually has is what it costs to get listed, which is a different axis and needs its
own terms. No amount of `Freemium` on a row would answer it.

`Unknown` appears in both columns wherever the terms were not stated plainly on the
directory's own site, and it appears often. Guessing would have filled the table and made it
worthless. A wrong value is worse than an absent one.



## Ordering

Alphabetical within a category, ignoring punctuation and a leading "The". Position carries no
meaning and there is no paid placement.

Between categories, the order is editorial, by expected reader interest. That ranks topics,
never products.

## Categories

Minimum 4 entries, 8 is the working target, roughly 15 is the ceiling. A category that cannot
reach 8 strong entries is merged or dropped rather than padded. No subcategories.

The taxonomy is revisited when a category drops below 6 entries, passes 15, or starts
receiving the same submissions as its neighbour.

## Links

The primary link is the resource's own official site: canonical, HTTPS, no tracking
parameters, no affiliate parameters, no shortener, no directory listing, no review page.

TiorAI links are capped: at most 25% of entries carry one, all distinct, at most three per
category, maintainer-placed only. Contributors are asked not to add them.

## Removal

An entry is removed when the product shuts down, the domain is taken over or starts serving
something harmful, the listing turns out to be misleading, or the entry no longer meets the
scope above. Removals are recorded in [CHANGELOG.md](../CHANGELOG.md). An entry removed for
a safety reason goes through review again rather than being quietly restored.
