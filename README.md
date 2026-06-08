# The SEO Agent. A full SEO workflow as a Claude Code skill.

Run your entire SEO program from one prompt, inside your own Claude. Audit your site, research real buying-intent keywords, plan a month of content, and write a finished, fact-checked article. Free, open source, no account needed to start.

> Built by [The SEO Agent](https://www.theseoagent.ai), the AI SEO agent that grows traffic on autopilot.

---

## What it does

Point your Claude at this skill and it runs the boring parts of SEO for you:

1. **Audits your site.** Pulls your pages and flags what is missing: titles, meta descriptions, H1s, thin content, weak internal links.
2. **Researches keywords.** Expands your topics into 50+ real buying-intent keywords, scores them by intent and opportunity, and clusters them into content themes.
3. **Plans 30 days of content.** A dated calendar of specific article titles, ordered by opportunity.
4. **Writes a finished article.** Picks your highest-opportunity title and drafts a complete, fact-checked, publish-ready post.
5. **Hands you a dashboard.** A single self-contained HTML file with your audit, your keywords (sortable, exportable to CSV), your calendar, and the sample article.

All of it runs in your own Claude. We charge nothing and see nothing.

## Quickstart

You need [Claude Code](https://www.claude.com/product/claude-code) (or any agent with web access, like claude.ai). Then:

```bash
git clone https://github.com/jeremy665/AI-SEO-Agent.git
cd AI-SEO-Agent
claude
```

Then tell Claude:

```
Run the SEO agent in PROMPT.md for my site: example.com
```

That is it. Claude reads `PROMPT.md`, asks you two or three quick questions about your business, and produces your dashboard. No key, no signup, no cost for the steps above.

Prefer to run a single skill? Point Claude at any file under `skills/` (for example `skills/site-audit/SKILL.md`).

## The suite

| Skill                 | Free, in your own Claude                                           | Paid, on autopilot                                                           |
| --------------------- | ------------------------------------------------------------------ | ---------------------------------------------------------------------------- |
| **Site audit**        | Flags missing titles, meta, H1s, thin content, weak internal links | Deep audit: real backlinks, competitor gaps, live rankings, AI-content score |
| **Keyword research**  | Autocomplete expansion + intent scoring (estimated volume)         | Real search volume and difficulty from live data, fully scored               |
| **Content writing**   | Drafts one finished article                                        | Writes and ships a ranking article every day, hands-off                      |
| **Content review**    | Reviews and fact-checks a draft you paste in                       | Production quality gate on every published piece, at scale                   |
| **Backlink swaps**    | Finds relevant swap candidates                                     | A real backlink exchange network of vetted businesses                        |
| **Native publishing** | Exports clean Markdown and HTML                                    | One click to WordPress, Webflow, Shopify, Wix, or Ghost                      |

The free column is genuinely useful and costs you nothing but your own Claude usage. The paid column is the stuff that needs real data, real publishing integrations, and a real network. See [`theseoagent/SKILL.md`](theseoagent/SKILL.md) for exactly what each tier unlocks.

## Honest about the free tier

We are an SEO company that hates SEO tricks, so we will be straight with you:

- The free keyword volumes are **estimates** derived from Google Autocomplete and search signals, not a paid data provider. They are directionally right, good enough to plan with, and clearly labeled as estimates. Real monthly volume and keyword difficulty need a live data API.
- The free skill writes **one** article and stops. It does not publish to your site, it does not run on a schedule, and you have to run it again by hand every time.

That gap is the point. Doing real keyword research, writing a good article, fact-checking it, and publishing it to your CMS, every single day, is a part-time job. The free skill shows you it can be done well. [The SEO Agent](https://www.theseoagent.ai) does it for you, on a schedule, connected to your site, for a flat price.

## Unlock the rest

When you want real data, daily auto-writing, and one-click publishing:

1. **Sign up free** at [theseoagent.ai](https://www.theseoagent.ai/signup) and copy your API key from Settings.
2. Drop it into `.env` as `THESEOAGENT_API_KEY` (see [`.env.example`](.env.example)).
3. Start your trial for **$1** (3 days, then $99/mo, one click to cancel in-app). Your first real article goes live in minutes.

Simple pricing. Real cancellation. No tricks.

## Why trust an AI to do this

The same reason you are already using Claude Code: a good agent does the grind, you keep the judgment. The SEO Agent runs real keyword research before it writes, cites its claims, fact-checks before publishing, and refuses to ship a draft that does not pass its own quality gate. It is an [AI SEO agent](https://www.theseoagent.ai), not an article spinner.

## License

MIT. Fork it, change it, ship it. See [`LICENSE`](LICENSE).

---

Made by the team behind [The SEO Agent](https://www.theseoagent.ai). One keyword in. One ranking post out.
