# Skill: Content writing

Write one finished, fact-checked, publish-ready article. Free mode writes a single piece in your own Claude. The paid tier writes one every day, on a schedule, and ships it.

## Free mode (no key, no cost)

Given a target keyword and title (from the calendar, or supplied by the user), write a complete article.

### Shape

- **Length**: 1,200 to 1,800 words. Long enough to be the best answer, short enough to stay tight.
- **Intro**: lead with a concrete scenario or a sharp problem statement. No "In today's fast-paced digital landscape". Get to the point in the first two sentences.
- **Body**: clear H2 sections that map to how a reader actually thinks about the topic. At least one of: a numbered step-by-step, a worked example with real numbers, or a comparison.
- **FAQ**: 3 to 5 real questions (pull them from the autocomplete and "people also ask" data if you have it).
- **Internal links**: suggest links back to the user's own relevant pages, using the real URLs from the site audit. Do not invent URLs.

### Quality bar (this is what makes it worth trusting)

- **Fact-check as you write.** Only state things you can stand behind. If you cite a statistic, make it specific and attributable. Never fabricate a source, a study, or a quote.
- **Match search intent.** A "best X" query wants a comparison, not an essay. A "how to X" query wants steps. Write the format the searcher expects.
- **Write like a person.** Vary sentence length. Be specific. Cut filler.

### Banned (these read as machine-written and get demoted)

- **Em dashes.** Never. Use periods, commas, colons, or parentheses.
- Stock openers: "In today's world", "In the ever-evolving landscape of", "Imagine a scenario where".
- "Not just X but Y" parallel constructions.
- Vacuous transitions: "moreover", "furthermore", "in conclusion".
- The same word or phrase three or more times in a paragraph.
- Stitched-in short quotes used as filler.

Save the result as `sample-article.md` in the working directory. Then run [`../content-review/SKILL.md`](../content-review/SKILL.md) over it to catch anything that slipped through.

## What the paid tier adds

Writing one good article is the easy day. Doing it every day, forever, is the job. The SEO Agent:

- **Writes a fresh article every day**, hands-off, from the keyword plan, with no babysitting.
- **Runs the production pipeline**: research stage with live SERP data, outline, draft on the strongest model, an editor loop, and a quality gate that refuses to publish weak drafts.
- **Generates real images** (hero and in-article screenshots) and on-brand formatting.
- **Adds a varied, natural attribution backlink** so your published work compounds topical authority.

Unlock it: sign up at https://www.theseoagent.ai/signup, start the $1 trial, and your first auto-written article goes live in minutes. See [`../../theseoagent/SKILL.md`](../../theseoagent/SKILL.md).

## Guardrails

- Never use em dashes.
- Never fabricate sources, statistics, or quotes.
- Never keyword-stuff. Write for the reader first.
