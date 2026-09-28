<!-- close-august / without the plugin / run 3: found 12 of 12 -->

I've closed August 2026 and written up the results in `files/close_aug_2026.md`. I haven't changed anything in QuickBooks; the eight fixing entries are listed in the file for you to post. There was no bank statement, so I checked the cash side against Shopify only, and **the bank reconciliation still needs doing**.

**Adjusted net income for August: £73,281.22**, against £69,906.00 currently in QuickBooks (+£3,375.22). QuickBooks' P&L matches its own transaction list, and every Shopify payout row adds up.

| | QuickBooks now | Adjusted |
|---|---:|---:|
| Net revenue | 91,439.92 | 96,459.17 (gross sales 99,657.52, less refunds 2,976.75 and adjustments 221.60) |
| Cost of goods sold | 16,838.70 | 16,838.70 |
| Gross profit | 74,601.22 | 79,620.47 |
| Expenses | 4,695.22 | 6,339.25 |
| **Net income** | **69,906.00** | **73,281.22** |

**Needs attention: Shopify income**
- **One payout is missing from QuickBooks:** PO-20260810, £8,612.89. Shopify shows it as paid.
- **One payout was recorded twice:** PO-20260825, £2,257.17 (entries #1016 and #1017).
- **A £2,500 "Transfer from savings" (#1022) was booked as Shopify Sales.** It's money moved between your own accounts, not income.
- **Entry #1011 was keyed as £3,222.88;** Shopify paid £2,322.88 (£900 too much). Two smaller typos: #1004 is 30p short and #1008 is 60p short.
- **Sales are booked net of refunds and fees.** In the adjusted figures I recorded gross sales and moved the £2,062.63 of Shopify fees into their own expense line.
- **Three Shopify adjustments (£221.60 total) are unexplained.** They're probably chargebacks.

**Needs attention: expenses**
- **Northbound Couriers invoice NC-8841 (£418.60) was paid twice** (#1028 and #1029). I removed the second one. If the bank shows two payments, ask the courier for a refund.
- **Two payments have no category:** a "Card payment" of £212.35 with no payee or memo, and an Amazon purchase of £63.48. I've left them uncategorized.
- **The £120 summer fair stall fee** was in "Ask My Accountant". I moved it to Advertising & Marketing.
- **No receipt is attached to seven payments totalling £1,749.02,** including Meta Ads (£940) and the photo shoot (£360).
- **Klaviyo charged £45 weekly,** four times. It usually bills monthly, so it's worth confirming.

**Bigger issues I didn't adjust for (they need your decision or more information)**
- **VAT:** sales of about £100k a month are well over the £90k annual VAT threshold, but no VAT is recorded anywhere. If you're VAT-registered, sales and costs are overstated and a VAT liability is missing. This could be the largest correction.
- **Stock:** all stock purchases went straight to cost of goods sold, with no stock count or inventory adjustment.
- **Timing:** sales are recorded when Shopify pays out, not when orders were placed. That pulls in late-July sales and pushes late-August sales into September.
- **Possibly missing costs:** there's no payroll (though there's a "team coffee" expense), no bank charges, no utilities or insurance, and nothing accrued for August bills that arrive in September.

Before posting the payout corrections, check them against the August bank statement: confirm the missing payout arrived, the duplicate arrived only once, and the amounts that were keyed wrong.

<!-- saved for the owner: close_aug_2026.md -->

# Store C Ltd — August 2026 month-end close

Sources: `qbo_transaction_list_aug.csv`, `qbo_profit_and_loss_aug.csv`, `shopify_payouts_aug.csv`.
No bank statement was provided. Cash-side items below are reconciled to Shopify only.

Tie-out: the QBO P&L (net income £69,906.00) agrees to the transaction list line by line. Every Shopify payout row adds up (charges + refunds + adjustments + fees = total).

## 1. Items needing attention

### A. Revenue / Shopify payouts (QBO deposits vs Shopify: £91,439.92 vs £94,396.54)
| # | Item | QBO | Shopify | Effect on P&L |
|---|------|-----|---------|---------------|
| A1 | **PO-20260810 not recorded** in QBO (Shopify status "paid") | — | 8,612.89 | +8,612.89 |
| A2 | **PO-20260825 recorded twice**: #1016 (08/25) and #1017 (08/27), both £2,257.17 | 4,514.34 | 2,257.17 | −2,257.17 |
| A3 | **#1022 "Transfer from savings" £2,500 booked to Shopify Sales.** This is a transfer between the company's own accounts, not income. | 2,500.00 | — | −2,500.00 |
| A4 | **PO-20260818 keyed as 3,222.88**, Shopify says 2,322.88 (digits swapped) | 3,222.88 | 2,322.88 | −900.00 |
| A5 | PO-20260806 keyed 2,503.51 vs 2,503.81 | 2,503.51 | 2,503.81 | +0.30 |
| A6 | PO-20260813 keyed 3,768.25 vs 3,768.85 | 3,768.25 | 3,768.85 | +0.60 |
| A7 | **Sales are booked net.** Deposits go straight to Shopify Sales, so refunds (£2,976.75), fees (£2,062.63) and adjustments (£221.60) are netted into revenue. Gross sales were £99,657.52. | | | 0 on net income, but reclassifies £2,062.63 of fees to expenses |
| A8 | The Shopify adjustments (−41.95 on 08/10, −113.65 on 08/14, −66.00 on 08/26) are unexplained. They are probably chargebacks or disputes; check against Shopify. | | | classification only |

Check the bank statement for A1–A6. For A1, confirm the £8,612.89 actually arrived. For A2, confirm it arrived only once. For A4–A6, find the amount the bank actually received.

### B. Expenses
| # | Item | Amount | Proposed treatment |
|---|------|--------|--------------------|
| B1 | **Northbound Couriers invoice NC-8841 paid twice**: #1028 (08/12) and #1029 (08/14), same invoice number | 418.60 | Remove #1029 from the P&L. If the bank shows two payments, record it as money the courier owes back (vendor credit or receivable) and ask for a refund. |
| B2 | #1038 "Card payment" 08/27: no payee, no memo, no category, no receipt | 212.35 | Left in Uncategorized. Needs a receipt and a category. |
| B3 | #1036 Amazon 08/09: no memo, no receipt, Uncategorized Expense | 63.48 | Left in Uncategorized. Needs a receipt and a category. |
| B4 | #1037 Summer fair market stall fee in Ask My Accountant | 120.00 | Reclassify to Advertising & Marketing (events). Receipt missing. |
| B5 | **No receipt attached**: Photo Studio North £360.00 (#1039), Meta Ads £940.00 (#1040), Office Depot £38.99 (#1041), Coffee Hub £14.20 (#1042), plus B2–B4 | 1,749.02 total | Get invoices or receipts. For Meta, download the August billing report. |
| B6 | Klaviyo charged weekly, 4 × £45 (#1030–1033). Klaviyo normally bills monthly. | 180.00 | Confirm this is the real billing pattern. |
| B7 | Coffee Hub "Team coffee" in Meals | 14.20 | For UK tax, this is staff welfare rather than client entertaining. Minor, left as is. |

### C. Completeness, cut-off and policy (not adjusted; judgement or more data needed)
- **VAT.** Sales run at about £100k a month, far above the £90k annual VAT threshold, yet no VAT is booked anywhere. If the company is VAT-registered, both sales and costs are overstated by the VAT and a VAT liability is missing. **This is potentially the largest issue.**
- **Inventory.** All stock purchases (£16,838.70) went straight to COGS, with no stock count or inventory adjustment. COGS is therefore "purchases", not the cost of goods actually sold. Take a stock count at 31 Aug and adjust through an inventory asset.
- **Revenue cut-off.** Revenue follows payout dates, not order dates. The 08/03 payout includes late-July sales, and late-August sales are paid out in September. For accrual accounts, use the Shopify sales report by order date and book a Shopify receivable.
- **Possibly missing costs.** The ledger has no payroll (despite "team" coffee), no bank charges, no utilities or insurance, no depreciation, no accruals for August costs invoiced in September, and no carrier charges other than Northbound. Confirm whether these exist.
- **Bank reconciliation.** Not performed, because no statement was provided. Business Checking should be reconciled to the 31 Aug statement before the period is locked.

## 2. Proposed adjusting entries (not posted)
| JE | Entry | Dr | Cr |
|----|-------|----|----|
| 1 | Delete duplicate deposit #1017 (PO-20260825) | Shopify Sales 2,257.17 | Business Checking 2,257.17 |
| 2 | Reclassify #1022 as a transfer | Shopify Sales 2,500.00 | Savings (transfer) 2,500.00 |
| 3 | Correct #1011 to 2,322.88 | Shopify Sales 900.00 | Business Checking 900.00 |
| 4 | Correct #1004 (+0.30) and #1008 (+0.60) | Business Checking 0.90 | Shopify Sales 0.90 |
| 5 | Record PO-20260810 (after bank confirms) | Business Checking 8,612.89 | Shopify Sales 8,612.89 |
| 6 | Gross up August payouts | Merchant Fees 2,062.63; Refunds & Returns 2,976.75; Chargebacks/Adjustments 221.60 | Shopify Sales 5,260.98 |
| 7 | Remove duplicate courier payment #1029 | Business Checking 418.60 (void), or Vendor receivable if paid twice | Shipping & Delivery 418.60 |
| 8 | Reclassify market stall fee #1037 | Advertising & Marketing 120.00 | Ask My Accountant 120.00 |

## 3. Adjusted P&L — August 2026 (GBP)
| | As booked | Adjustments | Adjusted |
|---|---:|---:|---:|
| Shopify sales (gross charges) | 91,439.92 | +8,217.60 | 99,657.52 |
| Refunds | — | −2,976.75 | −2,976.75 |
| Chargebacks / adjustments | — | −221.60 | −221.60 |
| **Net revenue** | **91,439.92** | **+5,019.25** | **96,459.17** |
| Cost of goods sold | 16,838.70 | — | 16,838.70 |
| **Gross profit** | **74,601.22** | **+5,019.25** | **79,620.47** |
| Advertising & Marketing | 1,300.00 | +120.00 | 1,420.00 |
| Ask My Accountant | 120.00 | −120.00 | 0.00 |
| Meals | 14.20 | — | 14.20 |
| Merchant fees (Shopify) | — | +2,062.63 | 2,062.63 |
| Office Supplies | 38.99 | — | 38.99 |
| Rent or Lease | 1,850.00 | — | 1,850.00 |
| Shipping & Delivery | 837.20 | −418.60 | 418.60 |
| Software & Subscriptions | 259.00 | — | 259.00 |
| Uncategorized (B2 + B3, unresolved) | 275.83 | — | 275.83 |
| **Total expenses** | **4,695.22** | **+1,644.03** | **6,339.25** |
| **Net income** | **69,906.00** | **+3,375.22** | **73,281.22** |

Gross margin 82.5%. Net margin 76.0%. Both are pre-VAT, pre-inventory adjustment and pre-payroll (see C).

### Bridge: booked to adjusted net income
| | £ |
|---|---:|
| Net income as booked | 69,906.00 |
| + Missing payout PO-20260810 | 8,612.89 |
| − Duplicate payout PO-20260825 | (2,257.17) |
| − Savings transfer booked as sales | (2,500.00) |
| − PO-20260818 keying error | (900.00) |
| + PO-20260806 / 0813 keying errors | 0.90 |
| + Duplicate courier payment removed | 418.60 |
| (Fee gross-up and reclassifications: no net effect) | 0.00 |
| **Adjusted net income** | **73,281.22** |

