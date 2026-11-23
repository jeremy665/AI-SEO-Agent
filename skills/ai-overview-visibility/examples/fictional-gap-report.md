# AI Overview visibility gap report

> Worked format example only. Copper Finch, `copperfinch.example`, every cited source, every URL, every excerpt, and every finding in this file are fictional. The `.example` domains are reserved for documentation. This file is not live probe evidence.

## Scope

| Field | Value |
|---|---|
| Target | Copper Finch, `copperfinch.example` |
| Topic | Proposal and billing software for small architecture studios |
| Buyer | Owners and operations leads at architecture studios with 2 to 20 staff |
| Surface | Google AI Overview, read with a browser tool (fictional example) |
| Locale | Australia, English, desktop |
| Synthetic run date | 2026-07-30 |
| Questions approved | 18 |
| Question approval | Approved in the fictional run before probing |
| Live-site approval | Not requested and not granted |

## Executive summary

- Copper Finch was cited on 3 questions.
- It was named without a citation on 1 question.
- It was absent from the inspectable citation set on 9 completed probes.
- No AI answer appeared on 3 questions.
- Two probes failed and remain unknown.
- Confirmed citation rate: 3 of 13 answer-present probes with inspectable citations, or 23 percent.
- The strongest recurring gap is not article length. Cited pages answer the exact buyer question early, expose decision attributes in tables or steps, and cover architecture-specific billing entities that Copper Finch's pages either bury or omit.

The citation rate excludes no-answer and failed probes. The brand mention without a source stays in the denominator as a completed citation-verifiable probe, but it is not counted in the citation numerator.

## Status definitions

| Status | Meaning in this report |
|---|---|
| cited | An attached source link resolved to `copperfinch.example` and the source page contained a supporting excerpt |
| mentioned_not_cited | The answer named Copper Finch, but no attached source resolved to its domain |
| not_cited | The answer and its citations were inspectable, the probe completed, and the target domain was absent |
| no_ai_answer | The query completed and the tested surface showed no AI answer |
| probe_failed | The query or evidence capture did not complete reliably, so citation status is unknown |

## Per-question citation status

| ID | Approved buyer question | Status | Sources attached to the answer | Target page | Short diagnosis |
|---|---|---|---|---|---|
| Q01 | What is the best proposal software for a small architecture firm? | cited | T01, S01, S02 | `copperfinch.example/architecture-proposals` | Target gives a direct category answer. Roundups add comparison criteria and alternatives. |
| Q02 | Which architecture proposal software includes a fee calculator? | not_cited | S01 | `copperfinch.example/architecture-proposals` | Fee calculations appear only inside a long feature tour on the target page. |
| Q03 | How should an architecture studio compare proposal software? | not_cited | S01, S02 | `copperfinch.example/architecture-proposals` | Cited pages expose a decision table with architecture-specific fields. |
| Q04 | Which tools combine architecture proposals and invoicing? | cited | T01, S01 | `copperfinch.example/architecture-proposals` | Target states the proposal-to-invoice workflow directly and is extractable. |
| Q05 | What is the best way to turn an architecture proposal into an invoice? | not_cited | S03 | `copperfinch.example/billing` | Cited page gives a numbered five-step workflow before its product list. |
| Q06 | What software handles retainer billing for architecture firms? | not_cited | S03, S04 | `copperfinch.example/billing` | Target uses generic recurring-billing language and never names retainer drawdown. |
| Q07 | How can architects track reimbursable expenses for clients? | not_cited | S04 | `copperfinch.example/billing` | Cited page defines reimbursable categories and approval evidence. |
| Q08 | What is a good architecture invoice approval workflow? | no_ai_answer | none | `copperfinch.example/billing` | No AI answer appeared, so no citation winner is claimed. |
| Q09 | What billing software fits a five-person architecture studio? | mentioned_not_cited | S01, S02 | `copperfinch.example` | Copper Finch appeared in answer text, but only roundup pages were linked as sources. |
| Q10 | Should architects use industry billing software or general invoicing software? | not_cited | S02, S03 | `copperfinch.example/billing` | Target lacks a category comparison and the criteria that make the choice useful. |
| Q11 | How much should billing software cost for a small architecture firm? | not_cited | S05 | `copperfinch.example/pricing` | Target shows plan prices but not cost by studio size, project count, or billing workflow. |
| Q12 | Which architecture proposal tools include e-signatures? | cited | T02, S06 | `copperfinch.example/esignatures` | Target directly names the buyer, action, and signature audit trail. |
| Q13 | How should architects bill for approved scope changes? | no_ai_answer | none | `copperfinch.example/billing` | No AI answer appeared, so the report records an opportunity, not a loss. |
| Q14 | Can architecture invoice follow-up be automated? | probe_failed | unknown | `copperfinch.example/billing` | The answer surface timed out twice. Citation status remains unknown. |
| Q15 | Is there one tool for architecture proposal templates and billing? | not_cited | S01, S03 | `copperfinch.example/architecture-proposals` | Target has both features but no single answer block that connects them. |
| Q16 | What invoice software works for residential architects? | no_ai_answer | none | `copperfinch.example/billing` | No AI answer appeared on the tested surface. |
| Q17 | Can an architecture firm adopt billing software without changing accounting systems? | not_cited | S07 | `copperfinch.example/integrations` | Target lists integrations but does not answer the migration-risk question. |
| Q18 | How does an architecture studio switch from spreadsheets to billing software? | probe_failed | unknown | `copperfinch.example/integrations` | Search returned no usable answer evidence. It is not counted as not cited. |

## Synthetic source evidence registry

Every citation ID in the table above maps to an exact fictional URL and a short fictional source excerpt. In a real run, these fields must come from the live answer link and fetched source page.

### T01

- URL: `https://copperfinch.example/architecture-proposals`
- Observed update date: 2025-10-14
- Verbatim source excerpt: "Copper Finch turns an architecture proposal into a client-ready scope, fee schedule, acceptance record, and draft invoice in one workflow."
- Used by: Q01, Q04

### T02

- URL: `https://copperfinch.example/esignatures`
- Observed update date: 2026-06-18
- Verbatim source excerpt: "Architecture studios can send a proposal for signature, record the signer and timestamp, and keep the accepted scope beside the billing plan."
- Used by: Q12

### S01

- URL: `https://studioops.example/guides/architecture-proposal-software`
- Observed update date: 2026-07-01
- Verbatim source excerpt: "For a small architecture firm, compare proposal tools on fee calculation, reusable scope sections, e-signature, change tracking, and whether an accepted proposal can become an invoice without re-entry."
- Used by: Q01, Q02, Q03, Q04, Q09, Q15

### S02

- URL: `https://practicebuyer.example/reviews/architecture-studio-software`
- Observed update date: 2026-06-27
- Verbatim source excerpt: "A five-person studio usually needs role-based review, fixed-fee and hourly billing, reimbursable tracking, and a clean export to its existing accounting ledger."
- Used by: Q01, Q03, Q09, Q10, Q11

### S03

- URL: `https://practicebuyer.example/guides/proposal-to-invoice-workflow`
- Observed update date: 2026-07-09
- Verbatim source excerpt: "A reliable proposal-to-invoice workflow has five steps: approve scope, lock the fee basis, create billing milestones, record changes, and issue the invoice from approved work. For retainer work, apply each approved invoice against the retainer balance."
- Used by: Q05, Q06, Q10, Q15

### S04

- URL: `https://studiobackoffice.example/architecture/reimbursables-and-retainers`
- Observed update date: 2026-05-22
- Verbatim source excerpt: "Track printing, travel, consultants, and permit costs as reimbursables, attach evidence, route exceptions for approval, and draw retainers against issued invoices rather than project revenue."
- Used by: Q06, Q07

### S05

- URL: `https://smallpractice.example/buyers-guide/architecture-billing-cost`
- Observed update date: 2026-07-04
- Verbatim source excerpt: "Evaluate total cost by staff seats, active projects, payment fees, accounting export, and the time required to rebuild proposals as invoices."
- Used by: Q11

### S06

- URL: `https://signflow.example/guides/architecture-proposal-esignature`
- Observed update date: 2026-06-30
- Verbatim source excerpt: "An architecture proposal signature record should bind the client, accepted scope, fee schedule, signer, and timestamp in one auditable event."
- Used by: Q12

### S07

- URL: `https://studiofinance.example/guides/billing-without-accounting-migration`
- Observed update date: 2026-07-12
- Verbatim source excerpt: "A studio can change its proposal and billing workflow without replacing accounting if the new system exports customers, invoice totals, taxes, and payment status to the existing ledger."
- Used by: Q17

## Cited-source frequency

| Fictional domain | Questions cited on | Count |
|---|---|---:|
| `studioops.example` | Q01, Q02, Q03, Q04, Q09, Q15 | 6 |
| `practicebuyer.example` | Q01, Q03, Q05, Q06, Q09, Q10, Q15 | 7 |
| `studiobackoffice.example` | Q06, Q07 | 2 |
| `smallpractice.example` | Q11 | 1 |
| `signflow.example` | Q12 | 1 |
| `studiofinance.example` | Q17 | 1 |
| `copperfinch.example` | Q01, Q04, Q12 | 3 |

The counts describe this fictional approved set only. They do not measure universal visibility.

## Recurring patterns

### 1. Cited pages answer the decision before describing features

Evidence: S01 starts with five comparison criteria. S03 starts with a five-step proposal-to-invoice workflow. Copper Finch's billing page opens with a product tour and does not state the workflow until its fourth section.

Observed difference: directness appeared on 8 of the 9 `not_cited` questions.

Inference: an early self-contained answer is easier to retrieve and quote. This is not proof that position alone caused selection.

### 2. Architecture-specific entities beat generic billing language

Evidence: S02 and S04 name fixed fees, hourly billing, reimbursables, retainer drawdown, approved scope, and accounting exports. The target billing page says "flexible billing" and "expense support" without those entities.

Observed difference: missing entity coverage affected Q06, Q07, Q10, Q11, and Q17.

### 3. Decision tables make the comparison extractable

Evidence: S01 presents fee calculation, e-signature, scope changes, and proposal-to-invoice as visible table columns. The target spreads the same features across tabs.

Observed difference: table structure affected Q02, Q03, Q09, and Q15.

### 4. Freshness and schema are supporting differences, not conclusions

Evidence: S01 shows an update date of 2026-07-01 and contains visible comparison rows represented by `Article` and `ItemList` JSON-LD. T01 shows 2025-10-14 and contains only product-level schema.

Inference: freshness and matching structured data may improve extractability, but this run cannot prove either caused the citations.

## Page-level fix list

| Priority | Target page | Questions | Required change | Impact | Effort | Why now |
|---:|---|---|---|---:|---|---|
| 1 | `copperfinch.example/architecture-proposals` | Q02, Q03, Q04, Q09, Q15 | Add a direct category answer and architecture-specific comparison table above the feature tour | 5 | M | Five approved questions, repeated directness and table gap |
| 2 | `copperfinch.example/billing` | Q05, Q06, Q07, Q10, Q17 | Rebuild the first half around proposal-to-invoice steps, retainers, reimbursables, and accounting continuity | 5 | M | Five high-intent questions and repeated entity gap |
| 3 | `copperfinch.example/pricing` | Q11 | Add a studio-size cost table and total-cost explanation | 3 | S | One strong price question, low implementation effort |
| 4 | `copperfinch.example/integrations` | Q17, Q18 | Add a no-accounting-migration answer and spreadsheet transition checklist | 3 | M | One confirmed gap and one failed probe to retest |
| 5 | new_page_required | Q13, Q14, Q16 | Draft a greenfield billing-workflow guide after these questions produce usable answer evidence | 2 | L | Current evidence is no-answer or failed, so priority stays lower |

Impact uses buyer intent, question coverage, and recurrence. Effort reflects the actual page work. It does not estimate search volume.

## Concrete rewrite plan for the top 3 pages

### Page 1: architecture proposals

- Current URL: `https://copperfinch.example/architecture-proposals`
- Target questions: Q02, Q03, Q04, Q09, Q15.
- Insert location: directly below the H1 and one-sentence product summary.
- Add a 60 to 80 word answer block that starts with the explicit subject "Architecture proposal software" and states who it is for, which decision it solves, and the five criteria a small studio should compare.
- Add a visible comparison table with these columns: fee calculation, reusable scope, e-signature, change tracking, proposal-to-invoice handoff, accounting export, and best-fit studio size.
- Add H2 sections that use the approved question language for fee calculation and combined proposal plus billing workflows.
- Replace "flexible workflow" with concrete architecture entities: fixed fee, hourly phase, reimbursable, retainer, additional service, and accepted scope.
- Refresh every product capability against the live product before changing the visible update date.
- Add `ItemList` schema only if the comparison rows remain visible in the page body and the markup matches them.
- Re-probe Q02, Q03, Q04, Q09, and Q15 on the same surface and locale after the page is live and indexed.

### Page 2: billing

- Current URL: `https://copperfinch.example/billing`
- Target questions: Q05, Q06, Q07, Q10, Q17.
- Replace the opening feature carousel with a five-step visible workflow: approved scope, fee basis, billing milestones, change record, and invoice issue.
- Follow it with two 50 to 70 word standalone answer blocks: one for retainer drawdown and one for reimbursable expenses.
- Add a decision table comparing architecture-specific billing with general invoicing across phase fees, hourly work, retainers, reimbursables, scope changes, and accounting export.
- State that accounting migration is not required only if the current integration behavior supports that claim. Link to the verified integrations page.
- Add a worked example using a fictional project fee, approved change, reimbursable, and invoice. Label every amount as an example.
- Use `HowTo` schema only if the five steps are visible, complete, and correctly represented in the markup.
- Re-probe Q05, Q06, Q07, Q10, and Q17 after indexing.

### Page 3: pricing

- Current URL: `https://copperfinch.example/pricing`
- Target question: Q11.
- Insert location: below the plan cards.
- Add a 50 to 70 word direct answer to "How much should billing software cost for a small architecture firm?" Do not claim an industry average without a source.
- Add a table for 2-person, 5-person, and 15-person studios showing the real plan, seats, active-project limits, payment fees, and included accounting exports.
- Add a total-cost checklist: subscription, payment fees, setup time, data migration, proposal re-entry, and accounting handoff.
- Keep `SoftwareApplication` or offer schema aligned with the visible current prices. Do not add review or rating fields without genuine user-review evidence.
- Re-probe Q11 after the pricing page is live and indexed.

## Validation

| Check | Result |
|---|---|
| Approved questions reconcile to all statuses | pass, 18 total |
| Every claimed citation maps to an exact synthetic URL and source excerpt | pass |
| Failed probes are separate from not-cited results | pass |
| No-answer queries claim no citation winner | pass |
| Evidence and inference are labeled separately | pass |
| Fixes use only verified target URLs or `new_page_required` | pass |
| Live site modified or published | no |
| API key required | no |

## Approval Gate 2 state

Not requested. This example ends with local rewrite instructions. No live page was changed or published.
