---
title: SEO Audit — findings
key: 1kbupkk1
---

# DTC SEO Audit — smokerolla.com

**Market:** United States · **Data:** Ahrefs (US) + a first-party crawl of all 122 collections, 28 pages, 30 blog URLs and the sitemap index. **Date:** see this page's history.

## The headline number

| Metric | Value |
|---|---|
| Organic traffic (US, monthly est.) | **1,679** |
| Organic keywords | 444 (185 in top 3) |
| Products in sitemap | **3,909** |
| Collections | 122 |
| Blog URLs | 224 |
| Paid traffic | 0 (restricted category — expected) |

**3,909 products generate ~1,679 visits/month.** For scale, four competitors in the same niche pull 25k–106k monthly US visits on similar or smaller catalogs.

## Finding 1 — Your traffic rests on a handful of blog posts, not on the store

Traffic by page type, across the 357 keywords with volume ≥10:

| Page type | Keywords | Traffic | Share of traffic |
|---|---:|---:|---:|
| Blog posts | 169 | **1,547** | **77%** |
| Products | 160 | 340 | 17% |
| Home | 11 | 137 | 7% |
| Collections | 16 | **20** | **1%** |
| Pages | 1 | 0 | 0% |

A single post — [top-5-electric-weed-grinders](https://smokerolla.com/blogs/magazine/top-5-electric-weed-grinders) — carries **990 visits, 59% of the entire site's organic traffic**, on 86 keywords. Remove it and the site has ~690 visits.

**This is the core structural risk.** Your *commercial* pages — the 122 collections where people actually buy — earn **1% of organic traffic combined**. The content engine works; it just isn't attached to the store.

## Finding 2 — The collection pages are good, and they're not ranking

This surprised me. I expected thin, auto-generated Shopify collections. Instead the median collection has **4,545 characters** of real copy, a sensible H1, and a keyword-shaped title. `/collections/herb-grinders` has 8,202 characters, a buyer's guide, an FAQ block and 30 products. That's genuinely well-built.

They still don't rank. The reason isn't on-page quality — it's that **the blog posts outrank them for their own keywords**, and the collections have almost no external authority pointing at them. `ref_domains` on your top 40 pages has a **median of 0**.

So this is not a "write better collection copy" problem. It's an **authority and internal-linking** problem.

## Finding 3 — 43 keywords, 215,470 combined volume, where you already have the right page

The highest-leverage list on the site. These are keywords a competitor ranks for, where **you already own a matching collection** but sit outside the top 10:

| Volume | Your page | Body | Products shown | Top keyword |
|---:|---|---:|---:|---|
| 45,000 | `/collections/dab-rigs-oil-rigs` | 6,758 ch | 28 | dab rig |
| 27,350 | `/collections/dry-herb-vaporizers` | 3,650 ch | **5** | dry herb vaporizer |
| 25,200 | `/collections/nectar-collectors-straws` | 6,912 ch | 29 | nectar collector |
| 25,000 | `/collections/vape-pens` | **3,492 ch** | **8** | vape pen |
| 20,000 | `/collections/herb-grinders` | 8,202 ch | 30 | weed grinder |
| 13,700 | `/collections/electric-dab-rigs` | 3,861 ch | **8** | electric dab rig |
| 9,300 | `/collections/terp-slurpers` | 5,123 ch | 14 | terp slurper |
| 8,300 | `/collections/glass-blunts` | 3,509 ch | **2** | glass blunt |
| 7,400 | `/collections/bongs-water-pipes` | 7,664 ch | 28 | water bong |
| 4,800 | `/collections/ash-catchers` | 4,037 ch | 11 | ash catcher |

Note the pattern in the **Products shown** column: `dry-herb-vaporizers` surfaces **5 products** for a 26,000-volume keyword; `glass-blunts` surfaces **2**; `vape-pens` **8**. **35 of 122 collections show fewer than 10 products.** A collection page with 2 products is a weak commercial result no matter how good the copy is — and Google's product-grid expectations for these queries are 20+.

## Finding 4 — You're on page 2–3 for keywords you should own

Ranking 11–30 means the page is understood and just under-powered. Cheapest wins available:

| Keyword | Volume | Position | KD | Page |
|---|---:|---:|---:|---|
| pink bong | 2,300 | 27 | 0 | `/collections/cute-and-girly-bongs...` |
| best grinder | 1,700 | 11 | 33 | blog: top-5-electric-weed-grinders |
| wax vape | 1,000 | 29 | 0 | `/collections/best-wax-vaporizers-oil-vapes` |
| girly bongs | 1,000 | 30 | 43 | `/collections/cute-and-girly-bongs...` |
| best blunt wraps | 800 | 16 | 0 | `/frequently-asked-questions-faqs` |
| blunt wrap | 600 | 27 | 0 | blog: blunt-wraps-101 |
| pink bongs | 600 | 25 | 0 | `/collections/pink-bongs` |
| cheap bongs under $25 amazon | 450 | 27 | 0 | `/collections/pipes-under-25` |

Several of these have **KD 0**. Position 25–30 at KD 0 almost always means a page that exists but has no internal links and no authority — not a hard fight.

**Also note the cannibalisation:** "pink bong" (2,300) points at `/collections/cute-and-girly-bongs...` while "pink bongs" (600) points at `/collections/pink-bongs`. Two pages splitting one intent; neither wins.

## Finding 5 — Index bloat from seasonal and operational collections

**19 seasonal/ops collections are indexable in your sitemap**, most padded with the same 23-product boilerplate:

`4th-of-july-sale` · `cinco-de-mayo` · `world-cup-special` · `fathers-day-collection` · `father-s-day-gifts` · `spooky-stash-halloween` · `happy-7-10` · `spring` · `end-summer` · `summer-daze` · `come-back-sale` · `veterans-day-collection` · `25-off-cannabis-accessories-event` · `smooth-selection-fresh-finds` (653 ch, 0 products) · `quick-order` · `sitewide-collection` · `volume-deal-eligible` · `dropshippable-items` (950 ch, 0 products) · `cannabis-accessory-vendors-shop`

Two problems: they dilute crawl budget across a 4,284-URL site, and `dropshippable-items` / `cannabis-accessory-vendors-shop` are **B2B pages sitting in the DTC index** — wrong audience, and they compete with your own wholesale subdomain.

## Finding 6 — Smaller on-page items

- **38 of 122 titles exceed 60 characters** — truncated in the SERP. Includes money pages like `/collections/dab-rigs-oil-rigs`.
- **9 collections have a missing or under-70-character meta description.**
- **79 of 122 collections have no FAQ block**; 88 have no buyer's guide. The ones that do (herb-grinders, dab-rigs) are your best pages — the pattern is proven, just unevenly applied.
- **4 collections link zero products.**
- `/collections/electric-grinders` (1,896 ch, 7 products) and `/collections/electric-herb-grinders` (6,001 ch, 9 products) are **near-duplicates competing for the same term** — while your top-performing blog post targets exactly that keyword. Three-way cannibalisation on your single best topic.
- **Crawl note:** Shopify rate-limited the audit crawl aggressively (627 of 675 requests returned 429). Not an SEO issue in itself, but it does slow Googlebot on a 4,284-URL site.

## Correction — internal linking (revised after crawling all 224 blog posts)

**An earlier version of this audit said your blog posts don't link into the store. That was wrong** — a parsing error in my crawler stripped the article body before counting links. Corrected findings, from all 224 posts:

- **183 of 219 posts (84%) do link into collections.** Median **3 collection links** and **3 product links** per post. The internal-linking discipline is largely there.
- **36 posts (16%) have zero collection links**; 34 of those link no products either. Those are the ones to fix, not all 224.
- **75 of 122 collections receive at least one blog link. 50 receive none.**

Most-linked collections: `/vaporizers` (66 posts) · `/bongs-water-pipes` (55) · `/electric-dab-rigs` (49) · `/dabbing-accessories` (43) · `/cleaning-solution` (43).

**So the real problem is distribution, not absence.** Links are concentrated on a handful of collections while others get nothing — including money pages:

| Collection | Blog links | Volume at stake |
|---|---:|---|
| `/glass-blunts` | **0** | 8,300 (glass blunt) |
| `/pink-bongs` | **0** | 2,900 (pink bong/bongs) |
| `/gas-mask-bongs` | **0** | 3,400 |
| `/mushroom-bongs` | **0** | 2,000 |
| `/steamroller-pipes` | **0** | 200 |
| `/terp-slurpers` | 6 | 9,300 |
| `/ash-catchers` | 7 | 4,800 |
| `/nectar-collectors-straws` | 15 | 25,200 — your KD-0 top target |

Brand collections are almost all orphaned: `/puffco`, `/ooze`, `/raw`, `/g-pen`, `/arizer`, `/storz-bickel`, `/santa-cruz-shredder`, `/focus-v-carta`, `/mob-hookah`, `/weedgets` — **zero blog links each**. Given that brand hubs scored as your best opportunity on difficulty ([[smokerolla-dtc-seo/priority-shortlist]]), that's a direct, cheap fix.

The finding that still stands: these collections have a **median of 0 referring domains** externally. Internal links help distribute what authority you have; they don't substitute for external links.

## What I'd do, in order

1. **Fix product counts on the top 10 money collections.** `dry-herb-vaporizers` (5 products / 26k volume), `glass-blunts` (2 / 8.3k), `vape-pens` (8 / 25k), `electric-dab-rigs` (8 / 13.7k). Highest ratio of effort to reward on the site — merchandising, not writing.
2. **Redistribute internal links toward the orphans.** Not a site-wide rewrite — 84% of posts already link out properly. Target the **50 collections receiving zero blog links** (especially `/glass-blunts`, `/pink-bongs`, `/gas-mask-bongs` and the ten orphaned brand collections) and the **36 posts** that link nothing. Free, immediate, entirely under your control.
3. **Resolve the three cannibalisation clusters** — electric grinders (3 pages), pink/girly bongs (2), blunt wraps (blog vs FAQ page). Pick a canonical page per intent, 301 or de-optimise the others.
4. **Noindex the 19 seasonal/ops collections**, and move the two B2B ones off the DTC index entirely.
5. **Rewrite the 38 over-length titles** to under 60 characters.
6. **Roll out the FAQ + buyer's-guide pattern** from `herb-grinders` to the other money collections — it's already proven on your own site.

Items 1–5 are optimisation of what exists; none require new content. Item 6 does.

→ Keyword-level opportunity list: [[smokerolla-dtc-seo/content-gap]]

**Difficulty-scored view:** [[smokerolla-dtc-seo/priority-shortlist]] re-ranks the fix list by traffic potential ÷ difficulty.
