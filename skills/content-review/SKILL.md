# Skill: Content review

Catch the AI tells, unsupported claims, and keyword stuffing in a draft before it ships. Free mode reviews a draft you paste in. The paid tier runs this gate automatically on every published piece.

## Free mode (no key, no cost)

Given a draft (the user pastes it, or you point at a `.md` file), review it on these axes and return a marked-up version plus a short verdict.

### 1. AI-tell scan

Flag and rewrite each instance:

- **Em dashes.** Replace every one with a period, comma, colon, or parentheses.
- **Stock openers**: "In today's fast-paced world", "In the ever-evolving landscape", "Imagine a world where".
- **"Not just X but Y"** parallel constructions.
- **Vacuous transitions**: "moreover", "furthermore", "in conclusion", "it is worth noting that".
- **In-paragraph repetition**: the same keyword or phrase three or more times in one paragraph.
- **Stitched-in short quotes** used as filler rather than evidence.

Give the draft an AI-tell verdict: human, mixed, ai-heavy, or fully-ai, with the specific evidence that drove it.

### 2. Fact and claim check

- Find every factual claim, statistic, and named source.
- Mark anything that is unsupported, vague ("studies show"), or likely fabricated.
- Suggest either a specific attributable source or a rewrite that drops the unverifiable claim.

### 3. Intent and structure check

- Does the article match what the target keyword's searcher wants (comparison vs how-to vs explainer)?
- Is there a real intro hook, scannable H2s, and at least one concrete example or list?
- Is the keyword used naturally, not stuffed?

### 4. Output

Return: the cleaned draft, a bullet list of what you changed and why, and the AI-tell verdict.

## What the paid tier adds

Reviewing one draft by hand is fine. Guaranteeing every published piece passes, at volume, is the product. The SEO Agent runs this as a hard **quality gate** inside the pipeline:

- Every article is scored before it can publish, and the agent **refuses to ship** drafts that fail.
- The same AI-tell ban list is enforced programmatically, with floors the model cannot talk its way under.
- Claims are fact-checked against the research stage's real sources.

Unlock it: sign up at https://www.theseoagent.ai/signup. See [`../../theseoagent/SKILL.md`](../../theseoagent/SKILL.md).

## Guardrails

- Never use em dashes (including in your own notes back to the user).
- Be specific about what you flag. Quote the offending text.
