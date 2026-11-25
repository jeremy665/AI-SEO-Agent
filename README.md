# AI SEO Agent: free SEO skills for AI coding agents

Install every skill with one line:

```bash
npx skills add jeremy665/AI-SEO-Agent
```

Install one check on its own:

- AI Overview check: `npx skills add jeremy665/AI-SEO-Agent --skill ai-overview-visibility`
- Core update check: `npx skills add jeremy665/AI-SEO-Agent --skill core-update-check`

Add `-g` to install for all your projects. Works in Claude Code and the other agents the skills CLI supports. No account and no API key.

## Start here: does Google's AI answer cite your site?

`ai-overview-visibility` checks whether Google's AI Overview, the AI answer at the top of the results, cites your site when buyers search the questions that come before a purchase. When it does not, it shows which pages are cited instead and what they do that your pages do not.

1. It reads your site and writes 15 to 25 real buyer questions for your topic. Then it stops so you can approve, edit or cut them.
2. It searches each approved question and records the AI answer and the sources linked to it. Every citation comes with the exact URL and a short quote from that page.
3. It compares the cited pages with yours: format, how directly they answer, structure, what they cover, freshness, schema, and how easy the answer is to lift out.
4. It writes a gap report with page fixes ranked by impact and effort, plus rewrite instructions for your top pages.

A search that failed or did not load is reported as failed, never as "not cited". It never edits your site.

To read Google's AI Overview, your agent needs a browser tool. Without one, it asks you to search each question and paste the AI answer back. It can also check your agent's own web search answer, which it always labels as a separate source and never as Google.

Try it:

```text
Use the ai-overview-visibility skill to check example.com for "proposal software for architects".
```

A full worked report for a made-up company: [fictional-gap-report.md](skills/ai-overview-visibility/examples/fictional-gap-report.md).

## Core update check: what helps or hurts your site in a Google core update

`core-update-check` audits a live website against what Google's core updates reward and punish, using only your public sitemap and fetched HTML.

1. It reads `robots.txt` and your sitemap to map your pages, spot publishing bursts or off-topic sections, and pick a real cross-section of 12 to 20 pages (plus any dropped URLs you name).
2. It fetches each live page and checks seven areas: technical and indexation blockers, duplicate titles and metadata, scaled low-value content and contradicted claims, first-hand evidence, depth for longer multi-part questions, topic hubs and internal links, and site-wide trust signals.
3. If you paste a Google Search Console export or use your own Search Console connection, it checks before and after clicks with a built-in small-sample noise check so normal swings on a small site do not get misread as a penalty.
4. It writes `core-update-check-report.md`: a per-page scorecard, four triage buckets (fix now, merge or prune, strengthen, keep), and concrete rewrite instructions for your top pages.

Every finding cites the exact URL and quotes what is on the live page. It never guesses rankings or traffic, never claims an "AI percentage" score, and never edits your site.

Try it:

```text
Use the core-update-check skill to check example.com.
```

A full worked report for a made-up company: [fictional-core-update-report.md](skills/core-update-check/examples/fictional-core-update-report.md).

## The other skills

| Skill | What it does |
| --- | --- |
| `seo-workflow` | One full pass: site audit, keyword research, a 30-day plan, one finished article, and an HTML dashboard with a CSV export. |
| `seo-site-audit` | Checks titles, meta descriptions, H1s, thin pages and internal links on your live site, with the URL for every fix. |
| `seo-keyword-research` | Finds buying-intent keywords with Google Autocomplete and web search. Volumes are estimates and labelled as such. Can use your own Search Console data. |
| `seo-content-writing` | Writes one fact-checked article, ready to publish, in the format the search calls for. |
| `seo-content-review` | Reviews a draft for AI tells, unsupported claims and keyword stuffing, and returns a cleaned version. |
| `seo-backlink-swaps` | Finds relevant sites to approach for a link swap or guest post, with a contact path for each. |
| `seo-article-export` | Turns an article into clean Markdown, HTML and the SEO fields to paste into your CMS. |

Every skill is free. Each one runs on your own agent with its own web tools, and none of them calls our servers or a paid API. Each skill's instructions are in `skills/<name>/SKILL.md`, so you can read exactly what it will do before you install it.

## The paid product

These skills do the work once, by hand. [The SEO Agent](https://www.theseoagent.ai/?utm_source=skill&utm_medium=github&utm_campaign=ai-seo-agent&utm_content=readme) does it every day: keyword research from real search data, one fact-checked article a day, and publishing to WordPress, Webflow, Shopify, Wix, Ghost, Framer or a webhook. [Start for US$1](https://www.theseoagent.ai/onboarding?utm_source=skill&utm_medium=github&utm_campaign=ai-seo-agent&utm_content=readme-start). That covers three days and your first 3 articles for new accounts. Then it is US$99 a month, and you can cancel in the app.

## License

MIT. See [LICENSE](LICENSE).
