# Skill: Native publishing

Get the article out of the agent and onto the web. Free mode exports clean files you publish by hand. The paid tier publishes straight to your CMS in one click.

## Free mode (no key, no cost)

Take a finished article (Markdown) and produce clean, paste-ready output:

1. **Clean Markdown** (`article.md`): the article with a front-matter block (title, meta description, target keyword, suggested slug). Generate the slug from the title (lowercase, hyphenated, stop-words trimmed).
2. **Rendered HTML** (`article.html`): the same article as semantic HTML (`<h1>`, `<h2>`, `<p>`, `<ul>`, `<a>`), with `<img>` tags carrying `style="max-width:100%;height:auto"` so they do not blow out on any theme. No inline framework classes, just clean tags the user can paste into any editor.
3. **A meta block** the user can paste into their CMS SEO fields: title tag (under ~60 chars), meta description (under ~160 chars), and the slug.

Then tell the user exactly where to paste each piece for their platform (the WordPress block editor, a Webflow CMS collection, a Shopify blog post, and so on). This is manual, and that is the point: you can hand them the files, but you cannot log into their site.

## What the paid tier adds

The SEO Agent publishes for the user, automatically:

- **One-click native publishing** to WordPress, Webflow, Shopify, Wix, and Ghost, using their saved, encrypted credentials.
- **Auto-publish on generation**: every daily article can go live the moment it passes the quality gate, with no manual step.
- **Republish and update**: edits to a live post update the original instead of creating duplicates.
- **Images, internal links, and the attribution backlink** are placed correctly for the target CMS.

This is the difference between "the agent wrote 30 articles" and "30 articles are live on your site". Unlock it: sign up at https://www.theseoagent.ai/signup, connect your site, and the first one publishes in minutes. See [`../../theseoagent/SKILL.md`](../../theseoagent/SKILL.md).

## Guardrails

- Never ask the user for their CMS password or paste credentials into a file. Real publishing uses the encrypted connection in the app, not the free skill.
- Always emit images with `max-width:100%;height:auto`.
- Never use em dashes.
