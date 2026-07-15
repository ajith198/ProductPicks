# Categories & expansion strategy

**Status: multi-category, as of 2026-07-12. Updated 2026-07-14.** ProductPicks started as a pickleball-only site (see `niche.md` for that original research). This file governs the site now that it has expanded into multiple product verticals, and is the doc future automated/daily runs should consult when choosing what to write next.

## Front matter taxonomy

Every post must set three custom front matter fields in addition to Jekyll's own `categories:` (which only controls the URL and should stay lowercase/hyphenated, e.g. `[footwear, buying-guides]`):

```yaml
category: Sports          # top-level vertical — see "Active categories" below
subcategory: Pickleball   # the specific gear type within that vertical
```

`date:` already supplies the year for the search UI — no separate year field is needed.

These two fields drive the Category / Type / Year filters in the search bar on the homepage (`_includes/guide-search.html`). Forgetting them doesn't break the build, but the post won't be filterable, so always set both.

## Active categories

| Category | Subcategories covered so far |
|---|---|
| Sports | Pickleball, Soccer, Tennis, Cycling, Running |
| Home & Kitchen | Coffee Makers, Electric Kettles, Blenders |
| Outdoor & Recreation | Camping Tents, Sleeping Bags, Headlamps, Hiking Boots |

New subcategories can be added freely within an existing category. New top-level categories should only be added when there's a genuine cluster of buyer-intent content planned for it (not a one-off post) — keep the category list short enough that the dropdown filter stays useful.

## Choosing what to cover next (the "data analysis" step)

Before writing a new subcategory, do the same lightweight analysis `niche.md` did for pickleball — no live data feed is wired up, so this is researched judgment, not a scraped dashboard:

1. **Buyer intent** — does the product category have clear, high-intent search phrases ("best X for beginners", "X vs Y")? Avoid categories where people mostly browse rather than research-before-buying.
2. **Amazon Associates eligibility** — no restricted categories (supplements, health-claim products, adult items, anything requiring ungating).
3. **Competition** — prefer categories not already dominated by large-budget authority sites (Wirecutter, RTINGS, etc.) for the specific long-tail keywords being targeted.
4. **Evergreen runway** — does the category support many future long-tail posts (skill levels, budget tiers, use-case splits, head-to-head comparisons), not just one post?

## Daily output target

Each day's actual output is governed by that day's automation task instructions, not by this file — the task has specified one new post per day in recent runs. Spread subtopics across categories/subcategories rather than piling onto one, and always check `content-log.md` first to avoid repeating a subtopic already covered.

## Format conventions (unchanged from the original niche)

- Same voice/structure as existing posts: affiliate-disclosure line at the top, a "what actually matters" spec-education section, then bolded/linked product picks as their own paragraphs (this renders as a callout card via the CSS in `assets/css/main.css`), a decision framework, and a "verify before you buy" checklist.
- All affiliate links use `config/affiliate.md`'s current tracking placeholder/ID.
- Approximate prices only, always caveated to check the live listing.
