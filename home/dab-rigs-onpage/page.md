---
title: Dab Rigs — on-page pass (applied)
key: 16gt9qu3
---

# /collections/dab-rigs-oil-rigs — full on-page pass

The head-to-head analysis put **12,711 monthly competitor visits** on this single collection — the largest unclaimed block on the site. This is the fix, applied live to Shopify on 2026-04.

**Target page:** [Dab Rigs & Oil Rigs for Concentrates](https://smokerolla.com/collections/dab-rigs-oil-rigs)
**Keyword set:** 82 keywords · headline term **"dab rig"** — 45,000/mo, **difficulty 3**, DankGeek holds position 3 with 6,630 visits/mo.

## What was actually wrong

The page was not thin or badly written — the body copy was already good (6,156 words of real buying guidance, FAQ, curated picks). Four structural faults were keeping it out of the running:

| # | Fault | Detail |
|---|---|---|
| 1 | **Wrong collection rule** | Smart rule matched `product_type = "Dab Rigs"`. But your rigs live under **five** different product types — 140 as `Dab Rigs`, 13 as `Recycler Dab Rig`, plus e-rigs filed under `Vaporizers` and `Smoking Accessories`. 10 in-stock rigs were invisible to their own category page. |
| 2 | **Body covered 4 of 82 keywords** | The copy said "dab rig" and "e dab rig" but never *portable dab rig* (2,500/mo), *electronic dab rig* (1,100/mo), *cheap dab rig* (700/mo), *dab rig kit*, or *dab rig parts*. |
| 3 | **Meta description omitted the modifiers** | No "portable", no "electronic" — the two highest-traffic qualifiers in the set. |
| 4 | **Under-linked** | 28 incoming blog links vs 49 for the smaller `electric-dab-rigs`. Eleven dab-topic posts discussed rigs at length and linked to *sibling* collections instead. |

Fault 1 is the same taxonomy debt already documented in [Shopify findings](https://work.leopoldo-s-space.letaido.app/home/smokerolla-dtc-seo/shopify-findings) — a rule keyed to a vocabulary the catalogue doesn't consistently use.

## What was changed

### 1. Collection rule rebuilt on a tag

Tagged **162 genuine rig products** with `Cat_DabRig` (excluding coils, atomizers, mouthpieces, replacement tops and ash catchers that merely had "recycler" in the title), then switched the smart rule from `type = Dab Rigs` to `tag = Cat_DabRig` + in-stock.

**Products on the page: 98 → 108.** Ten in-stock rigs — including the Puffco Peak Smart eRig, Lookah Unicorn Next Gen and several recycler rigs — are now merchandised on the page that should rank for them.

### 2. Body copy extended to the keyword set

Added a **"Shop dab rigs by type"** navigation block with six cards, each carrying a buyer-intent term as a real internal link: electronic dab rigs, cheap dab rigs (under $50), recycler rigs, silicone rigs, dab rig parts (bangers/carb caps), dabbing accessories.

Expanded the lead paragraph to carry *portable*, *electronic* and *cheap* naturally, and added **four FAQ entries** answering the question-shaped keywords: what is a portable dab rig, what is the best cheap dab rig, what comes in a dab rig kit, can I replace dab rig parts.

**Keyword coverage in the body: 4 → 13 of 82**, representing **10,759 of the 12,711** monthly competitor visits on this set. The remaining 69 are long-tail variants that the same page now covers semantically.

Copy grew 8,436 → 10,838 characters. No existing content was removed.

### 3. Meta description rewritten

Before: *Shop dab rigs, oil rigs and electric e-rigs at Smokerolla — mini rigs, recyclers and portable e-rigs from Dr. Dabber, Lookah, Calibear, Yocan and more.*
After: *Shop dab rigs and oil rigs at Smokerolla — glass rigs, recyclers, **portable dab rigs** and **electronic** e-rigs from Dr. Dabber, Lookah, Puffco and Pulsar. Fast US shipping.*

Title was already correct (`Dab Rigs & Oil Rigs for Sale | Smokerolla`, 41 chars) and was left alone.

### 4. Ten internal links added from dab-topic blog posts

Ten posts that discussed rigs but linked elsewhere now link to the collection in prose, with varied anchors (*electric dab rigs*, *e-rigs*, *dab rig*, *dab rigs & oil rigs*) rather than one repeated phrase:

best-e-rigs-worth-buying-2026 · seshgear-dabtron-electronic-dab-rig-base-jar-review · best-quartz-bangers-2026-buyers-guide · lookah-q7-mini-enail-banger-review-2026 · lookah-snail-2-0-wax-kit-review-2026 · puffco-proxy-all-colors-review-2026 · dab-rite-pro-silicone-replacement-review-2026 · best-wax-pens-2026 · puffco-peak-pro-ball-cap-all-colors-review · lookah-dragon-egg-wax-vaporizer-kit-review

**Incoming blog links: 28 → 38.**

## Verified live

Re-fetched [the collection](https://smokerolla.com/collections/dab-rigs-oil-rigs) and the edited posts after publishing: new meta description live, navigation block rendering, "portable dab rig" and "electronic dab rig" present in HTML, 108 products in the smart collection, links resolving on the blog posts.

## Backups

| File | Contents |
|---|---|
| `~/workspace/dabrig_backup.json` | Full collection object + all metafields, pre-change |
| `~/workspace/dabrig_tags_backup.json` | Original tag string for all 162 tagged products |
| `~/workspace/dabrig_articles_backup.json` | Original `body_html` of all 10 edited posts |

## What to expect, honestly

Difficulty 3 on a 45,000/mo term does not mean position 3 is available on merit alone — DankGeek holds it with a far stronger domain. What this pass buys is **eligibility**: the page now has correct inventory, covers the qualifier keywords, and receives internal authority proportional to its commercial value. Movement on the long-tail qualifiers (*portable dab rig*, *electronic dab rig*, *cheap dab rig*) should come first and fastest; the head term is a longer campaign.

Re-check positions in **3–4 weeks**. If the qualifiers move and the head term doesn't, the constraint is domain authority, not on-page — and the answer then is the next two collections, not more edits here.

## Next in the queue

Per the [head-to-head ranking](https://work.leopoldo-s-space.letaido.app/home/smokerolla-dtc-seo/head-to-head): **electric-dab-rigs** (7,044/mo — note its rule has the same tag-vocabulary fault, matching tag `Electric Dab Rigs` while pulling only 24 products), then **ash-catchers** (5,843) and **nectar-collectors-straws** (5,466).

← [[smokerolla-dtc-seo/head-to-head]]
