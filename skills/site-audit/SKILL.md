# Skill: Site audit

Find what is holding a site back in search. Free mode runs entirely in your own Claude against the live site. The paid tier adds real off-page data (backlinks, competitors, rankings) that the public web does not hand you for free.

## Free mode (no key, no cost)

You have web fetch and shell. Use them.

1. **Enumerate the site's pages.**
   - Fetch `https://<domain>/sitemap.xml` and `https://<domain>/sitemap_index.xml`. Follow any nested sitemaps. Collect the URLs.
   - If there is no sitemap, fetch the homepage and collect internal links, then go one level deep.
   - Cap at the 10 to 20 most important pages (homepage, top-level sections, recent posts) so this stays fast.

2. **Inspect each page.** Fetch the HTML and record:
   - `<title>` (present? unique across pages? under ~60 chars?)
   - meta description (present? unique? under ~160 chars?)
   - first `<h1>` (present? exactly one?)
   - rough word count of the main content
   - whether the page links to other pages on the same site

3. **Detect single-page-app catch-alls before judging.** If two different routes return byte-identical HTML, the site is a client-rendered SPA. Say so, and do not claim "every page has a duplicate title". That is a rendering artifact, not an SEO bug.

4. **Report fixable issues, specifically.** For each finding, name the URL and the fix:
   - Missing or duplicate title tags
   - Missing meta descriptions
   - Missing or multiple H1s
   - Thin pages (under ~300 words of real content)
   - Orphan pages (no internal links pointing in)
   - Pages with no internal links out

Do not pad the list. Do not invent issues. A short, correct, specific list beats a long speculative one.

## What the paid tier adds

The free audit can only see on-page signals, because real off-page SEO data is not public. The deep audit at [theseoagent.ai](https://www.theseoagent.ai) pulls:

- **Backlink profile**: referring domains, link velocity, spam ratio, anchor distribution.
- **Competitor gap**: who outranks the site and for what, and which keywords are winnable.
- **Live rankings**: where the site actually sits in the SERP today.
- **AI-content score**: how machine-written the site's own content reads, with verbatim evidence, so the user can fix it before Google does.

To run it: sign up at https://www.theseoagent.ai/signup, then audit any domain from the dashboard. See [`../../theseoagent/SKILL.md`](../../theseoagent/SKILL.md).

## Guardrails

- Cite the URL for every finding.
- Never claim a ranking, backlink, or traffic number in free mode. You cannot measure those without paid data, so do not guess them.
- Never use em dashes.
