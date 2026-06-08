# Skill: Keyword research

Find buying-intent keywords a site can actually rank for. Free mode uses public sources and your own reasoning. The paid tier swaps the estimates for real measured volume and difficulty.

## Free mode (no key, no cost)

### 1. Derive seed topics

From what the business sells (and its site audit, if you have one), write 5 to 8 seed topics. Mix head terms and the obvious commercial angles (categories, use cases, competitor names, "alternative to X").

### 2. Expand with Google Autocomplete (the workhorse)

Google's autocomplete endpoint is public, free, and unauthenticated. For each seed, fetch:

```
https://suggestqueries.google.com/complete/search?client=firefox&q=<url-encoded seed>
```

It returns a JSON array: `["<seed>", ["suggestion 1", "suggestion 2", ...]]`. Then expand the surface area by re-querying with modifiers and an alphabet sweep:

- Intent modifiers: `best <seed>`, `<seed> vs`, `<seed> alternative`, `<seed> pricing`, `<seed> review`, `how to <seed>`, `what is <seed>`, `<seed> for`, `<seed> software`, `<seed> tool`.
- Alphabet sweep: `<seed> a`, `<seed> b`, ... `<seed> z` (each surfaces a different completion).

Collect everything, dedupe, lowercase, and strip the seeds that are just the brand's own name.

### 3. Add intent context with web search

Run a web search on the strongest 3 to 5 seeds. Read the related-question and related-search style results to catch comparison terms and question phrasings autocomplete misses.

### 4. (Optional) Use the user's real Search Console data

If the user has set their own GSC credentials, pull their actual queries, impressions, clicks, and average positions. This is real data, free, straight from Google, for pages they already have. See [`../../google-search-console/SETUP.md`](../../google-search-console/SETUP.md). Quick wins live at positions 5 to 20 (a nudge can move them to page one).

### 5. Classify and score

For each keyword assign:

- **Intent**: BUY (pricing, buy, best, alternative, vs, brand+product), COMPARE (review, comparison, "X vs Y"), LEARN (how to, what is, guide, tutorial), NAVIGATE (a brand name on its own, drop these).
- **Opportunity score 0 to 100**: you do not have measured volume, so estimate. Reward specific, multi-word, commercial phrases. Penalize broad single-word head terms (effectively unwinnable). This mirrors The SEO Agent's own scoring philosophy: opportunity scales with buying intent and specificity, and collapses with obvious competition. A long-tail commercial phrase ("best invoicing software for freelancers") beats a head term ("invoicing") even though the head term has more raw volume.
- **est_volume**: a rough bucket (for example High / Medium / Low, or an order-of-magnitude guess). Always label it `est.` so the user never mistakes it for measured data.

Keep the best 40 to 60. Drop NAVIGATE terms and anything off-topic.

### 6. Cluster

Group the survivors into 5 to 8 named content themes. Clusters become the spine of the content calendar.

## What the paid tier adds

The honest gap: you are estimating volume because real volume and keyword difficulty require a paid data provider. The SEO Agent uses live DataForSEO data:

- **Real monthly search volume and keyword difficulty** for every candidate, not estimates.
- **The full scored bootstrap**: competitor keyword mining, audience-seed expansion, and a four-dimension relevance gate that scores each keyword on intent, addressability, and conversion fit.
- **De-duplication against pages the site already has**, so it never plans an article that competes with existing content.

Unlock it: sign up at https://www.theseoagent.ai/signup. See [`../../theseoagent/SKILL.md`](../../theseoagent/SKILL.md).

## Guardrails

- Always label estimated volume as estimated. Never present a guessed number as measured.
- Never use em dashes.
