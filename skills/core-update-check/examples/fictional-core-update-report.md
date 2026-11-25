# Core update check report

> Worked format example only. Harborfield Ops, `harborfield.example`, every URL, quote, word count, and finding in this file are fictional. The `.example` domain is reserved for documentation. This file is not a live site audit.

## 1. Scope and limits

| Field | Value |
|---|---|
| Target domain | `harborfield.example` (field-service scheduling software for HVAC teams) |
| Synthetic run date | 2026-11-25 |
| Sitemap | `https://harborfield.example/sitemap.xml` (78 URLs listed) |
| Sampled URLs | 14 fetched (13 returned HTTP 200, 1 returned HTTP 404) |
| SPA catch-all check | Passed (distinct routes return distinct server-rendered HTML) |
| Search Console data | Not supplied |
| Live-site edits made | None |

What this free check cannot see: live Google rankings, real clicks or impressions, backlink counts, or user engagement. Every finding below comes strictly from the public sitemap and fetched HTML.

## 2. Executive verdict

**Observed core-update exposure across the sampled set: Moderate.**

Top three site-wide issues observed:
1. **Contradicted product claims on a core feature page:** `/features/route-optimization` claims "unlimited technician seats on every plan", while `/pricing` caps the Starter plan at 5 technicians.
2. **Publishing burst of thin, template-repeated city pages:** the sitemap shows 32 `/hvac-software/<city>` URLs carrying the same `<lastmod>` date (`2026-10-19`). Three sampled city pages run 210 to 245 words with identical paragraphs except the city name.
3. **Weak hub links and generic comparisons:** two sampled comparison pages lack concrete pricing/limit tables, quote no sources, and send zero internal links back to `/features/dispatch` or `/pricing`.

What the site already does well:
- Homepage, `/pricing`, and `/about` return clean server-rendered HTML with unique titles, clear team ownership, real customer-support contact details, and plain pricing.
- `/guides/hvac-dispatch-workflow` includes a worked 12-truck schedule example, real dispatch time numbers, and 6 contextual internal links.

## 3. Sitemap and publishing footprint

| Section | URLs in sitemap | `<lastmod>` pattern | Note |
|---|---:|---|---|
| Core product and pricing | 9 | Spread across 2026-03 to 2026-11 | Healthy update cadence |
| Guides and blog | 28 | 2 to 4 per month | 2 off-topic posts found (`/blog/best-office-chairs`, `/blog/free-invoice-spreadsheet`) |
| Comparisons (`/vs/*`) | 9 | 2026-08 to 2026-10 | Uneven depth across sampled pages |
| City pages (`/hvac-software/*`) | 32 | All 32 dated `2026-10-19` | Single-day burst; sampled pages are thin city-swapped templates |

## 4. Per-page scorecard

| URL | Status | Words | Title / Meta / H1 | First-hand proof | Links out | Main finding | Bucket |
|---|---|---:|---|---|---:|---|---|
| `/` | 200 | 740 | Clean, unique | Product UI specs, pricing | 14 | Clear above-the-fold positioning | Keep as is |
| `/pricing` | 200 | 510 | Clean, unique | Exact tier limits | 8 | Conflicts with `/features/route-optimization` | Keep as is (source of truth) |
| `/features/route-optimization` | 200 | 490 | Clean, unique | Generic claims | 4 | False claim: "unlimited technician seats on every plan" | Fix now |
| `/features/dispatch` | 200 | 680 | Duplicate meta desc | Concrete workflow | 7 | Shares meta description with `/` | Fix now |
| `/about` | 200 | 420 | Clean, unique | Named founders, office address | 6 | Strong trust signals | Keep as is |
| `/guides/hvac-dispatch-workflow` | 200 | 1,640 | Clean, unique | Worked 12-truck example | 6 | Strong hub candidate; missing visible update date | Strengthen |
| `/vs/ductflow` | 200 | 890 | Stale year ("2024") in title | None; generic summary | 1 | No pricing table, no tradeoffs, 1 internal link | Strengthen |
| `/vs/crewgrid` | 200 | 940 | Clean, unique | Mentions crew-size fit | 2 | Needs "who should skip us" section and verified table | Strengthen |
| `/hvac-software/austin` | 200 | 228 | Template title | None | 1 | Thin city-swapped copy from Oct 19 burst | Merge, redirect, or prune |
| `/hvac-software/dallas` | 200 | 219 | Template title | None | 1 | 88% identical copy to `/hvac-software/austin` | Merge, redirect, or prune |
| `/hvac-software/denver` | 200 | 241 | Template title | None | 1 | Same template skeleton; zero local specifics | Merge, redirect, or prune |
| `/blog/best-office-chairs` | 200 | 610 | Clean, unique | None; AI-tell opener | 0 | Off-topic filler unrelated to HVAC software | Merge, redirect, or prune |
| `/blog/hvac-maintenance-checklist` | 200 | 1,120 | Missing meta desc | Real seasonal checklist | 2 | Useful guide; add meta desc and links to hub | Strengthen |
| `/guides/dispatch-kpis` | 404 | 0 | N/A | N/A | 0 | Listed in sitemap and linked from `/features/dispatch` | Fix now |

## 5. Site-wide findings (Evidence vs Inference)

### Technical and indexation confounders
- **Evidence:** `https://harborfield.example/guides/dispatch-kpis` appears in `sitemap.xml` and is linked from `/features/dispatch`, but returns HTTP `404`. All 13 live pages have self-referencing canonicals and no accidental `noindex`.
- **Inference:** Leaving dead URLs in the sitemap and feature navigation wastes crawl effort and creates broken reader journeys.

### Metadata review and duplicate templates
- **Evidence:** `/features/dispatch` uses the exact same meta description as `/` ("Modern HVAC scheduling software built for growing teams."). `/vs/ductflow` has `<title>Harborfield vs DuctFlow (2024 Comparison)</title>`. `/blog/hvac-maintenance-checklist` has no meta description tag.
- **Inference:** Unreviewed or stale metadata weakens click clarity and signals neglected commercial pages.

### Scaled low-value content and unreviewed AI signals
- **Evidence:** `/features/route-optimization` states "Every plan includes unlimited technician seats" while `/pricing` states "Starter: up to 5 technicians". Three sampled `/hvac-software/<city>` pages (`austin`, `dallas`, `denver`) come from a 32-page single-day burst (`2026-10-19`), average 229 words, and repeat the same three paragraphs with only the city name swapped. `/blog/best-office-chairs` opens with "In today's fast-paced world of remote operations..." and contains 4 instances of "moreover" and "furthermore".
- **Inference:** Scaled thin templates with zero local differentiation and unreviewed off-topic posts carry the highest exposure under Google's scaled content abuse guidance.

### First-hand experience, complex questions, and internal linking
- **Evidence:** `/vs/ductflow` and `/vs/crewgrid` contain prose summaries with no feature-by-feature table, no stated date for competitor pricing, and no section explaining which team size should choose the alternative. `/blog/best-office-chairs` has 0 internal links; the 3 city pages have 1 link each (homepage only).
- **Inference:** Complex buyer comparisons need explicit tradeoffs, verifiable specs, and clear links into the product and dispatch hub to satisfy multi-part commercial queries.

## 6. Ranked fix list

| Priority | URL or scope | Bucket | Impact (1 to 5) | Effort | Exact change | Why now |
|---:|---|---|---:|---|---|---|
| 1 | `/features/route-optimization` | Fix now | 5 | S | Fix contradicted "unlimited technician seats" copy to match `/pricing` | False commercial claim on a core product page |
| 2 | `/guides/dispatch-kpis` (404) | Fix now | 4 | S | Restore the guide or 301 redirect to `/guides/hvac-dispatch-workflow` and remove from sitemap | Broken URL in sitemap and live product navigation |
| 3 | `/hvac-software/*` (32 city pages) | Merge, redirect, or prune | 5 | M | After confirming zero Search Console clicks/links, consolidate into one service-area hub or add real regional compliance/pricing data | Highest scaled-content risk on the site |
| 4 | `/vs/ductflow` and `/vs/crewgrid` | Strengthen | 4 | M | Update title year, add verified comparison table, tradeoffs, crew-size fit, FAQ, and links to `/features/dispatch` and `/pricing` | High-intent buyer pages missing complex-query depth |
| 5 | `/blog/best-office-chairs` | Merge, redirect, or prune | 3 | S | Confirm zero clicks/backlinks in Search Console, then prune and remove from sitemap | Off-topic unreviewed filler |
| 6 | `/features/dispatch` and `/blog/hvac-maintenance-checklist` | Fix now | 2 | S | Write unique meta descriptions and link checklist to `/guides/hvac-dispatch-workflow` | Quick metadata and hub hygiene |

## 7. Concrete fix instructions for the top 3 pages

### Page 1: `/features/route-optimization`
- **Current issue (quoted):** "Every plan includes unlimited technician seats with zero per-truck fees."
- **Exact fix:** Replace with the real limits from `/pricing` ("Starter covers up to 5 technicians; Growth covers up to 25; Enterprise supports custom fleet sizes").
- **Add first-hand proof:** Insert one worked 8-stop morning route example showing drive-time minutes before vs after route grouping (labelled clearly with real internal test data or marked as an illustrative example).
- **Verified internal links to add:** `/pricing`, `/features/dispatch`, `/guides/hvac-dispatch-workflow`.

### Page 2: `/vs/ductflow`
- **Current issue (quoted):** `<title>Harborfield vs DuctFlow (2024 Comparison)</title>`; body has zero pricing specs and 1 internal link.
- **Exact fix:** Update title to remove stale year and state the decision angle clearly. Add a 60-word direct verdict right under the H1 naming who fits Harborfield (5 to 25 truck residential HVAC teams) and who fits DuctFlow.
- **Add complex-question depth:** Add a visible comparison table (crew size fit, dispatch board, offline mobile app, accounting sync, setup time, starting price with date checked), a 4-question FAQ on migrating active customer histories, and verified internal links to `/pricing`, `/features/dispatch`, and `/features/route-optimization`.

### Page 3: `/hvac-software/*` city template cluster (32 URLs)
- **Current issue (quoted):** `/hvac-software/austin` (228 words) and `/hvac-software/dallas` (219 words) share 88% identical copy published on `2026-10-19`.
- **Exact fix:** Check 90-day Search Console clicks and inbound links for all 32 URLs first. Unless a city page has real local demand and genuinely distinct local content (regional licensing, seasonal demand, local case details), consolidate the thin templates into one strong `/features/dispatch` or regional overview page and remove the unclicked stubs cleanly after any active rollout ends.

## 8. Search Console next step

No Search Console data was supplied for this run. Before pruning any URL:
- Compare equal 14-day windows before and after the latest completed rollout in Search Console (Pages report).
- If a page or site averages under 30 clicks a day, treat percentage swings carefully as small-sample noise rather than a confirmed penalty.
- Keep any page that earns steady non-branded clicks or real conversions; prioritize fixes on pages that actually lost clicks or carry false claims.

## 9. Validation summary

| Check | Result |
|---|---|
| Every sampled URL verified live or marked `fetch_blocked` | pass (13 HTTP 200, 1 HTTP 404) |
| Client-rendered SPA check performed before metadata grading | pass |
| No fabricated traffic, ranking, backlink, or AI-percentage numbers | pass |
| Observed evidence separated from inference | pass |
| Live site modified or published | no |
| Paid API or server called | no |
