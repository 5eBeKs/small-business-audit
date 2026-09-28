# A good free plugin, and what the owner still can't see

Anthropic's Small Business plugin for Claude, run on synthetic books and stores.

**Sample case · synthetic data · an independent check, not affiliated with or endorsed by Anthropic.**

Anthropic publishes a free [Small Business plugin](https://github.com/anthropics/knowledge-work-plugins/tree/da38ec1/small-business)
for Claude: 44 skills for closing the month, reports, payroll, taxes, invoices and more, written as
instructions (no scripts: the model writes its own code each time). Many small businesses will install
it rather than pay for skills of their own, and on this evidence they are right to: on synthetic books
with twelve planted problems it found every one, kept its receipt and duplicate rules in every run, and
left a tidy packet each time.

This case asks what it cannot do by design, as no general plugin can: know how *this* business counts.
Where an answer rests on a rule the owner never gave, the plugin picks one, often says which, and keeps
it once it is saved. But the first pick is the model's, and a fresh start can pick another; the
arithmetic is right either way. I ran it with Opus 5.5, three runs per question (five for the tax
phrasings), and kept every answer.

## In short

**What it does well**

- **Closing August on books with 12 planted problems:** all 12 found in every run, a spreadsheet, a
  PDF and a page each time, and its receipt and duplicate rules kept in every run: a 14.20 coffee not
  chased for a receipt (its rule starts at 25), a weekly plan not called a duplicate. Its 0.50 rule held
  less well: a 0.30 difference was noted as under it in all three runs, but one run also said to correct
  it, and all three put the 0.30 into the corrected figures, as plain Claude did. Plain Claude also found
  all 12, but with no rules to keep it asked for the coffee receipt in all three runs, questioned the
  weekly plan in two and treated the 0.30 as an error in all three.
- **The nine owner questions of my bench, with its skill called by name:** 25 of 27 right by the
  bench's automatic checks, 26 if a refund split the owner's definitions do not settle is accepted
  (my skills 27, plain Claude 26). `report-builder` says what it counted, saves the rules it used, and,
  rerun from a saved definition, followed it 6 of 6 times.
- **Routing, when the owner uses its words:** the intended skill in 29 of 30 sessions on ten
  phrasings, and its own tax rule held in 27 of 28 tax requests.

**What the owner still cannot see, or did not choose**

- **Which revenue.** Told not to wait (see section 1), each close pointed out that sales are booked
  net, then picked its own revenue for the corrected P&L: 94,396.54, 96,459.17 and 96,680.77 in three
  runs, one of them called only "net sales". Net income was 73,281.22 in all of them.
- **Which orders count.** On the same export one run counted an order tagged "test" and two left it
  out; two runs saved opposite rules for it in their report definitions, and neither asked first.
- **Whether the plugin ran at all.** Asked plainly with the export in the folder ("How did August
  go?", "Which of our products lost money?"), none of its skills ran in any of 27 routing sessions
  (these had no shell, and five stopped at four minutes still working) nor in one full session with a
  shell: the owner got plain Claude.

None of these is a bug to report. It is the part a general plugin cannot know about one business.

## Closing the gap, on top of the plugin

What I do for a business that uses this plugin, or skills of its own:

1. **Your rules, asked once.** Four questions (which revenue line, whether test orders are sales, when
   a sale counts, how a partial refund is split), answered in a file you can read, kept with the
   business context the plugin already stores, and printed under every figure.
2. **Checked on your exports.** Your recent months and a copy with planted problems, three runs each:
   every problem found, the same figure in every run, every order left out named.
3. **The way your people ask.** Routing tried on your own phrasings, so the right skill runs when
   someone asks "how did the month go?".
4. **The evidence handed over.** Every answer and every grade, as in this repository.

Fixed-price, quoted per export.

My own skills for these stores, on a similar bench, are in
[claude-skills-zoo](https://github.com/5eBeKs/claude-skills-zoo): the definitions printed under the
answer ("How this was counted") in 25 of 27 runs, 27 of 27 on versions 0.5.1 to 0.6.0, and every order
the owner should see named in 27 of 27. Contact: [Upwork](https://www.upwork.com/freelancers/ilyashkura).

## What was checked

| | |
|---|---|
| Plugin | `small-business` 1.35.1, [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins/tree/da38ec1) at `da38ec1`, Apache-2.0 |
| Model | Opus 5.5 only, three runs per question (five for the tax phrasings) |
| Sessions | `claude -p` in a fresh folder with the files; the close, bench-question and rerun sessions with a shell, the routing sessions with reading and skills only; no connectors (the plugin calls the CSV path "first-class"), no web, no user settings; the plugin loaded from a fresh copy |
| Start | cold: no onboarding (`smb-onboard`), not in Cowork, no business context stored |
| Data | synthetic: three Shopify stores (A in euros and B in dollars, an August export each, B's with three orders from 31 July; C in pounds, three months and 9,074 export rows) and store C's August books as QuickBooks Online exports them |
| Compared with | the same questions without any plugin, and with [my skills](https://github.com/5eBeKs/claude-skills-zoo) |

## 1. Closing August

Store C's August books: QuickBooks' transaction list and profit and loss, and Shopify's list of 21
August payouts ([`books/`](books/)). The owner's message:

> Please close August 2026 for us. [...] Don't wait on me to resolve anything: list everything that
> needs attention, then go all the way to the P&L summary. I'll deal with the flags afterwards.

That message overrides the plugin's own pauses: `month-end-prep` stops for the owner before its P&L
and `close-month` waits for the owner's sign-off. Every choice below was made because the owner said
not to wait.

With the plugin, `close-month` ran each time. The planted problems: a Shopify payout never entered in
the books (8,612.89), a payout entered with two digits swapped (900.00 off), one entered 0.60 short
(the plugin flags 0.50 or more), one entered twice, a "Shopify" deposit that is a transfer from savings,
a courier invoice keyed twice, three lines left uncategorized (Amazon, a market stall fee, a card
payment), and three more expenses over 25 with no receipt (a product shoot, ads, printer ink; the
uncategorized lines have none either).

| | With the plugin | Without |
|---|---|---|
| All 12 found, in the answer or the file the run saved | 3 of 3 runs | 3 of 3 runs |
| All 12 named in the chat answer itself | 3 of 3 | 2 of 3 (11 in the third) |
| The 14.20 coffee: under its 25 receipt rule | not chased in 3 | receipt asked for in 3 |
| The weekly 45.00 email plan: not a duplicate | not questioned in 3 | questioned in 2 (once as a possible duplicate) |
| The 0.30 difference: under its 0.50 threshold, "note but don't flag", in the text | noted in 3, also flagged in 1 | treated as an error in 3 |
| The 0.30 in the corrected figures | included in 3 | included in 3 |
| Time and what it left | 3.4 to 3.9 minutes; a spreadsheet, a PDF and a page | 56 to 108 seconds; a chat answer, and a Markdown file in two runs |

The run with the plugin that flagged the 0.30 gave its reason: payouts do not round, so 0.30 is more
likely a keying error than rounding. And every corrected P&L, with the plugin and without, books the
payouts at Shopify's payout amounts, 0.30 included (no bank statement was given): the threshold decides
what the owner is asked about, not the figures. Plain Claude has no rules to keep, and each of its choices is defensible too.

**The revenue line.** Every run turned the books into a corrected P&L: a pro forma the owner asked for,
beside the ledger's own P&L (91,439.92 of sales in every run). Shopify deposits are booked net of fees
and refunds, every run said so, and each chose its own way back to revenue:

| Run | With the plugin | Without |
|---|---|---|
| 1 | 96,459.17 ("net sales"; the fees moved to expenses, the basis not stated in words) | 96,680.77 (net sales: charges less refunds) |
| 2 | 94,396.54 (net payouts) | 96,459.17 (sales less refunds and adjustments) |
| 3 | 96,680.77 (before Shopify fees, after refunds; its packet calls it "corrected gross sales") | 96,459.17 (gross sales less refunds and adjustments) |
| Net income | 73,281.22 in all three | 73,281.22 in all three |

The plugin's `close-month` says "This step owns the numbers. Nothing later in the chain [...] restates
revenue." Within a run that holds; across runs, the pro forma revenue is 94 or 96 thousand depending on
the run, and which one the business reports is the owner's rule, not yet given.

## 2. The bench's questions

The nine questions my skills are tested on, word for word: how the month went (summary), where the money
went between sales and the bank (payouts), which products lose money (margins), on three stores. I
called the plugin's closest skill for each by name: `report-builder` for summary and margins,
`month-end-prep` for payouts. `month-end-prep` reconciles a ledger against the payment processor; the
payouts question gives orders and payouts, no ledger, so it is not an exact fit, and the plugin has no
skill for the bridge from orders to payouts. Its router is covered in section 3.

| Three runs per question, 27 per column | Small Business | My skills | Plain Claude |
|---|---|---|---|
| Right by the bench's automatic checks | 25/27 | 27/27 | 26/27 |
| ... accepting a refund split the owner's definitions do not settle | 26/27 | 27/27 | 26/27 |
| Every order or product the owner should see named, in the answer and saved text files | 19/27 | 27/27 | 21/27 |
| ... counting the plugin's own workbook sheets too | 21/27 | | |
| Store C, where the owner's definitions are in the folder: summary on them | 2/3 | 3/3 | 2/3 |
| ... payouts on them | 1/3 | 3/3 | 2/3 |
| Says it added the figures up by hand | 0/27 | 0/27 | 9/27 |

How these were read ([`results/bench-questions-table.md`](results/bench-questions-table.md)):

- The two columns on the right are this bench's earlier runs. On stores A and B they ran in `claude
  plugin eval`, which on Windows has no shell, and their judgement checks were decided by a model
  judge; the plugin's runs all had a shell, and its 12 judgement checks were decided by reading each
  answer, every verdict quoting the line it rests on ([`results/verdicts.json`](results/verdicts.json)).
  Plain Claude's 9 "by hand" answers are all on stores A and B, where it had no shell.
- "Named" uses the same coverage check for all three columns, against the list my skills' scripts give
  (orders left out and why, disputes, orders in transit, orders paid outside Shopify Payments, products
  below cost or with no cost). The plain-Claude runs kept only their answers and Markdown files, so
  the like-for-like row is the first; the plugin's workbooks are published sheet by sheet in
  [`answers/workbooks/`](answers/workbooks/), their copies of the raw export left out (a copy of the
  export names every order in it). Counting the workbooks, five of the plugin's six misses are on the
payouts question. A range
  such as "#1998–#2000" names every order in it. One plugin answer says "I matched it to MO-CND-001 by
  hand": a product code, not the figures, so it is not counted.

`report-builder` says to confirm the report's spec with the owner once before building it, and to ask
"only about what's genuinely ambiguous". None of its 18 runs stopped to ask before giving figures; one
said why: everything "could be worked out from your file". The two misses, read:

- **Store A, run 2** counted an order tagged "test" (59 orders, 2,999.72) where runs 1 and 3 left it
  out (58 orders, 2,918.82). It flagged the order and asked the owner to check it afterwards.
- **Store C, run 3** split partial refunds between goods and shipping in proportion to the order, and
  its revenue came out 14 pounds above the nearest reading the bench accepts. The owner's written
  definitions do not settle that split, so the second row counts it right; plain Claude's miss on
  store C is a real error (a total labelled as after discounts when it was before them, revenue
  about 1,000 pounds high).

**The saved definition.** `report-builder` writes each report's spec, formulas and rules to its own
`saved_reports.md` and, when it cannot, to `report-definitions.md` next to the owner's files. In these
unattended sessions Claude Code refused the edit of the plugin's file in 12 of the 18 runs ("a
sensitive file"), and the skill fell back as its instructions say; with one run that wrote both, 13
saved `report-definitions.md`. The other 5 appended to `saved_reports.md` through the shell (those
plugin copies were removed afterwards). The definition is where the test order
shows: store A's run 1 saved 'Voided orders and orders tagged "test" are excluded and listed', noting
#1013 as "excluded pending owner confirmation"; run 2 saved 'Orders tagged "test" are counted but
flagged for confirmation'. Asked for "the same report as last time" with each saved file next to the
same export, three times each, every rerun followed the rule its file held: 6 of 6
([`answers/rerun/`](answers/rerun/)). The mechanism works; what it keeps is whatever the first run
decided.

## 3. Routing

A fresh session per message, the plugin loaded, reading files and calling skills allowed (no shell),
and the first skill it called:

| The owner says | Skill called | Runs |
|---|---|---|
| Close the books for August. | close-month | 3/3 |
| Can you reconcile our August Shopify payouts against QuickBooks? | month-end-prep | 3/3 |
| Will I make payroll next month? | cash-flow-snapshot | 3/3 |
| What should I reorder this week? | inventory-planner | 3/3 |
| Get my documents together for taxes. | tax-prep 7, tax-season-organizer 1 | 3 + 5 |
| Build me a monthly sales report from our Shopify export. | report-builder | 3/3 |
| How's the business doing? | business-pulse | 3/3 |
| Who owes me money? | invoice-chase | 3/3 |
| I don't know where to start. | smb-router | 3/3 |
| Write a haiku about coffee. | none | 3/3 |
| Four more tax requests (quarterly, 1099s, books for the accountant, books already closed) | the plugin's rule each time | 20/20 |
| The bench's nine questions, the export in the folder | none | 27/27 |

The plugin's rule is that every tax request goes to `tax-prep` first, which checks the books are closed,
and to `tax-season-organizer` directly only when the owner says they are. One request in 28 skipped
that step. (`results/routing.json` accepts either tax skill for that phrasing and so counts 30 of 30;
by the plugin's own rule it is 29.) Five of the 27 bench-question sessions stopped at four minutes
while still working without a skill; one full session with a shell on store A's summary called none
either ([`results/routing-full-session.json`](results/routing-full-session.json)).

## 4. Static checks

`claude plugin validate --strict` passes on Claude Code 2.1.280 (it checks the manifests;
[`results/validate.txt`](results/validate.txt)). My linter finds two skills with a `version` field in
their frontmatter (accepted by the official validator) and two pairs of descriptions that overlap most:
`restock` and `inventory-planner` (routing picked `inventory-planner` 3 of 3), `tax-prep` and
`tax-season-organizer` (the one routing slip above). The style warnings it gives are my house rules,
not defects, and are not counted ([`results/lint.txt`](results/lint.txt)).

## What the plugin could change itself, in its own terms

1. **Ask the counting rules once and keep them, as it already does for country, currency and financial
   year** (`## Business context`: "Store the answer in the block so it is never asked again"): which
   revenue line the P&L reports (gross, after refunds, net of fees), whether an order tagged "test" is a
   sale, whether a sale counts when paid or when shipped, how a partial refund is split. Four
   questions, once, so that even an owner who says "don't wait" gets their own rule.
2. **Print that revenue definition next to the corrected P&L** in `close-month`, the step that "owns the
   numbers".
3. **Treat a paid order tagged "test" as the ambiguity `report-builder` Step 2 says to ask about**,
   rather than something that "could be worked out from your file".
4. **Let the plain questions reach the skills.** `report-builder` already says to "reach for it even when
   the owner names the metrics without using the word report"; "how did the month go" and "which
   products lose money" with an export in the folder could be named in its description.

## How to read this

- Run in September 2026. Synthetic data, Opus 5.5 only, three runs per question: a rate of 1 in 3 is a
  sign, not a measurement.
- The plugin ran cold, as an owner who skipped onboarding would have it: no `smb-onboard`, no stored
  business context, not in Cowork, in unattended `claude -p` sessions where a permission prompt is
  refused rather than asked. Onboarding does not ask the counting rules above, so the main finding
  stands; the refused edits of `saved_reports.md` are a feature of unattended sessions.
- The bench's checks were written for my skills; where a plugin answer used another defensible basis
  it was read, and each reading is recorded.
- A reply was ready for a skill that stopped to confirm its spec ("Looks right. Go ahead."); none of
  the 27 bench-question runs stopped, so it was never sent.
- No connector was used, and nothing here was reported to Anthropic as a bug.

## Files

- [`results/`](results/): routing, the close graded against the planted problems, the bench's questions
  with every check, the reader's verdicts, the reruns, the linter and the validator.
- [`answers/`](answers/): every answer as the owner read it, with the text files the runs saved:
  `close-august/`, `bench-questions/`, `saved-definitions/`, `workbooks/` (the bench questions'
  spreadsheets, one CSV per sheet), `rerun/`, and the full routing session. Not published: the close
  runs' spreadsheets and PDFs (their pages are in `packets/`), and the five definitions appended to the
  plugin's own file through the shell, whose plugin copies were removed.
- [`packets/`](packets/): the three close pages the plugin produced.
- [`books/`](books/): store C's August books and what a close must find (`ledger_truth.json`); the
  stores' orders are in [claude-skills-zoo](https://github.com/5eBeKs/claude-skills-zoo/tree/main/stores).

## License

My text, the readings and the synthetic data here are under [CC BY 4.0](LICENSE). The answers,
workbooks and packets are the plugin's and the model's output on that data; the packets use the
plugin's house style (`shared/reference/artifact-example.html`, Anthropic, Apache-2.0), and their links
to web fonts were removed on export. The plugin itself is Anthropic's, under Apache-2.0, and is not in
this repository; the lines quoted from it are marked as quotes.

Not affiliated with Anthropic, Shopify or Intuit.
