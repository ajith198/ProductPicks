# Today — 2026-07-12

## Site expansion: multi-category + search

Expanded ProductPicks from a pickleball-only site into a multi-category buying-guide site, and added a guide search/filter bar:

- Added `category` / `subcategory` front matter fields to every post (see `categories.md` for the taxonomy and active category list). Retrofitted the 2 existing pickleball posts with `category: Sports` / `subcategory: Pickleball`.
- Added a search bar at the top of the homepage guide listing (`_includes/guide-search.html`) with a text search plus Category / Type / Year dropdown filters, all client-side (no build step or external service needed).
- Updated `about.md`, `index.md`, `brand.md`, and `niche.md` to reflect the expansion; added `categories.md` as the authoritative doc for future runs on active categories and daily-output targets.

## New posts (5 today, across 3 categories)

1. "[Best Soccer Cleats for Beginners in 2026](/footwear/buying-guides/best-soccer-cleats-for-beginners/)" (Sports / Soccer)
2. "[Best Tennis Racquets for Beginners in 2026](/racquets/buying-guides/best-tennis-racquets-for-beginners/)" (Sports / Tennis)
3. "[Best Beginner Road Bikes Under $1,000 in 2026](/bikes/buying-guides/best-beginner-road-bikes-under-1000/)" (Sports / Cycling)
4. "[Best Drip Coffee Makers for Small Kitchens in 2026](/kitchen/buying-guides/best-drip-coffee-makers-for-small-kitchens/)" (Home & Kitchen / Coffee Makers)
5. "[Best 2-Person Backpacking Tents for Beginners in 2026](/outdoor-gear/buying-guides/best-2-person-backpacking-tents-for-beginners/)" (Outdoor & Recreation / Camping Tents)

## Post count

**7** posts published in `_posts/` (2 prior + 5 new today).

## Outstanding one-time human steps

1. **Enable GitHub Pages.** Go to the repo's Settings → Pages → Source: "Deploy from a branch" → select `main` (or `master`) → `/root`. This can't be done by the automation — it requires the GitHub UI. (Reminder will keep appearing until confirmed.)
2. **No Amazon Associates tracking ID yet.** All affiliate links in posts currently use the placeholder `AMAZON_AFFILIATE_LINK_PLACEHOLDER` (see `config/affiliate.md`). Once you're approved for Amazon Associates, add your real tracking ID to `config/affiliate.md` and future posts will start using it automatically. (Old posts with the placeholder will NOT be retroactively edited.)
3. **Amazon Associates / Google AdSense applications.** With 7 posts published, this is closer to (but still slightly under) the 10-15 post threshold both programs generally want to see before approving — hold off a few more days.
4. **Filesystem note:** `TODAY.md` and `today.md` are two different paths tracked in git, but on a case-insensitive filesystem (like this Mac) they resolve to the same file on disk, so only one actually exists locally. Not touched further in this run since it's a pre-existing repo state, but worth deciding which casing to keep and removing the other from git tracking at some point.

Next runs should keep adding at least 5 new buyer-intent posts per day, spread across categories per `categories.md`, and keep `content-log.md` up to date to avoid repeating subtopics.
