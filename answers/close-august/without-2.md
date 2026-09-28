<!-- close-august / without the plugin / run 2: found 12 of 12 -->

I've closed August 2026 on paper, but nothing is posted in QuickBooks yet. After my corrections, August net income is **£73,281.22**; QuickBooks currently shows £69,906.00. The full workpaper, with the flags, eight adjusting entries you can post in QuickBooks and the P&L, is in `aug_2026_close.md`. I couldn't reconcile the bank account because there's no bank statement among the exports.

**Shopify payouts compared with QuickBooks deposits.** Shopify paid out £94,396.54. QuickBooks shows £88,939.92 of payout deposits, and the gap of £5,456.62 is fully explained:
- The 10 Aug payout, PO-20260810 (£8,612.89), isn't in QuickBooks at all.
- The 25 Aug payout, PO-20260825 (£2,257.17), is entered twice: deposits #1016 and #1017.
- Deposit #1011 is £3,222.88, but the payout was £2,322.88, so it's £900 too high.
- Deposits #1004 and #1008 have small typos, together £0.90.

**Other errors I corrected in the adjusted figures:**
- A £2,500 "Transfer from savings" (#1022) is booked as Shopify sales. It's a transfer, not income.
- Northbound Couriers invoice NC-8841 (£418.60) is recorded twice (#1028 and #1029).
- Shopify income is recorded after refunds and fees were taken off. I split it out into sales £99,657.52, refunds £2,976.75, adjustments £221.60 and fees £2,062.63. This doesn't change net income.
- The £120 summer fair stall fee was in "Ask My Accountant". I moved it to Advertising & Marketing; that one is my call, so change it if it belongs elsewhere.

**Still open for you:**
- **No account or description:** a £212.35 "Card payment" (no payee, account or receipt) and a £63.48 Amazon charge (no memo). They stay uncategorized for now.
- **Shopify adjustments:** £221.60 across three payouts. They look like chargebacks, but that needs confirming in Shopify.
- **No receipt attached** (7 items, £1,749.02): Meta Ads £940, Photo Studio North £360, the card payment £212.35, the market stall fee £120, Amazon £63.48, Office Depot £38.99 and Coffee Hub £14.20.
- **VAT:** there are no VAT accounts at all, yet sales are running at about £97k a month, far above the UK registration threshold. Check whether you're VAT-registered and whether the Shopify figures include VAT.
- **Stock:** all stock purchases (£16,838.70) went straight to cost of goods sold, and there's no month-end stock count. The 83% gross margin needs checking against a count.
- **Unpaid bills:** the stock payments are coded to cost of goods sold rather than Accounts Payable. Check for open bills from the same suppliers so those costs aren't counted twice.
- **Timing:** sales are counted when Shopify pays out, not when the sale happened. Late-July sales fall in August, and sales from about 29–31 August fall in September.

**Adjusted P&L, August 2026:**

| | £ |
|---|---:|
| Net revenue (sales 99,657.52, less refunds and adjustments) | 96,459.17 |
| Cost of goods sold | 16,838.70 |
| **Gross profit** | **79,620.47** |
| Expenses (including 2,062.63 Shopify fees) | 6,339.25 |
| **Net income** | **73,281.22** |

The workpaper walks through the difference from QuickBooks line by line. The VAT, stock and timing points could change the result a lot, so treat £73,281.22 as provisional until they're resolved.

<!-- saved for the owner: aug_2026_close.md -->

# Store C Ltd: August 2026 month-end close

Sources: `files/qbo_transaction_list_aug.csv`, `files/qbo_profit_and_loss_aug.csv`, `files/shopify_payouts_aug.csv`.
The QBO P&L ties to the QBO transaction list. No bank statement was provided, so the bank has not been reconciled.
None of the entries below have been posted to QuickBooks.

## 1. Shopify payouts vs QBO deposits

Shopify paid out £94,396.54 in 21 payouts. QBO shows £88,939.92 of payout deposits, plus a £2,500 savings transfer that was coded to Shopify Sales.

| Payout | Shopify | QBO | Difference | Issue |
|---|---:|---:|---:|---|
| PO-20260810 | 8,612.89 | none | +8,612.89 | Payout missing from QBO |
| PO-20260825 | 2,257.17 | 4,514.34 (#1016 on 8/25, #1017 on 8/27) | -2,257.17 | Recorded twice |
| PO-20260818 | 2,322.88 | 3,222.88 (#1011) | -900.00 | Keying error (3↔2) |
| PO-20260806 | 2,503.81 | 2,503.51 (#1004) | +0.30 | Keying error |
| PO-20260813 | 3,768.85 | 3,768.25 (#1008) | +0.60 | Keying error |
| **Net** | | | **+5,456.62** | Matches the £94,396.54 − £88,939.92 gap exactly |

Each payout's lines (charges + refunds + adjustments + fees) add up to its total.

## 2. Items that need attention

**A. Errors, corrected in the adjusted P&L**
1. PO-20260810 (£8,612.89) is not in August's books. Check whether it was posted to July or September by mistake. Then add it.
2. Deposit #1017 (£2,257.17) duplicates #1016 for PO-20260825. Delete it. Its number is also out of sequence with #1018.
3. Deposit #1011 is £3,222.88, but the payout was £2,322.88. Correct it (−£900).
4. Deposits #1004 (+£0.30) and #1008 (+£0.60) have small keying errors.
5. Deposit #1022 (£2,500, "Transfer from savings") is named Shopify and coded to Shopify Sales. This is a transfer, not revenue. Move it to the savings account, or to director's loan/capital if that's where the money came from.
6. Northbound Couriers invoice NC-8841 (£418.60) is booked twice (#1028 on 8/12, #1029 on 8/14). If only one payment cleared the bank, delete #1029. If both cleared, move the second to a vendor receivable/credit. It is not an expense either way.
7. Shopify revenue is booked net of fees and refunds. The adjusted P&L grosses it up: sales £99,657.52, refunds £2,976.75, adjustments £221.60, fees £2,062.63. Net income doesn't change.

**B. Missing categories or explanations**
8. #1038 "Card payment" £212.35 has no payee, no account and no receipt. It shows as "Uncategorized".
9. #1036 Amazon £63.48 has no memo or receipt and is coded to Uncategorized Expense.
10. #1037 Market stall fee £120 ("Summer fair") is in Ask My Accountant. I moved it to Advertising & Marketing. Change it if it belongs elsewhere.
11. Shopify "Adjustments" total −£221.60 (PO-20260810 £41.95, PO-20260814 £113.65, PO-20260826 £66.00). These are probably chargebacks or dispute fees. Confirm in Shopify. Shown as a contra-revenue line for now.

**C. Receipts missing** (no attachment in QBO; £1,749.02 in total)
Photo Studio North £360.00 (#1039), Meta Ads £940.00 (#1040), Market stall fee £120.00 (#1037), Card payment £212.35 (#1038), Amazon £63.48 (#1036), Office Depot £38.99 (#1041), Coffee Hub £14.20 (#1042).

**D. Accounting policy and completeness questions (not adjusted)**
12. **VAT:** The books have no VAT accounts. Sales are running at about £97k a month, well above the UK registration threshold. Confirm whether you're VAT-registered and whether the Shopify figures include VAT. If so, revenue and costs are overstated by the VAT. The Meta Ads invoice may also need reverse-charge treatment.
13. **Inventory:** All £16,838.70 of stock purchases went straight to COGS, and there's no stock count. COGS here means purchases, not the cost of goods actually sold. The 83% gross margin should be checked against a month-end stock count.
14. **Stock payments:** The five stock payments are "Bill Payment (Check)" transactions coded to COGS, not Accounts Payable. Check the A/P aging for open bills from Rosewater, Glassjar or Botanica, so the same costs aren't counted twice.
15. **Cut-off:** Revenue is recognised on the payout date. The 3 Aug payout includes late-July sales, and sales from about 29–31 Aug are paid out in September. For accrual accounting, use the Shopify sales-by-date report.
16. **Bank reconciliation:** Not done, because there's no statement. Items 1–6 will show up there.

## 3. Proposed adjusting entries

| # | Entry | Debit | Credit | Amount |
|---|---|---|---|---:|
| AJE-1 | Record PO-20260810 | Business Checking | Shopify Sales | 8,612.89 |
| AJE-2 | Remove duplicate deposit #1017 | Shopify Sales | Business Checking | 2,257.17 |
| AJE-3 | Correct deposit #1011 | Shopify Sales | Business Checking | 900.00 |
| AJE-4 | Correct #1004 / #1008 | Business Checking | Shopify Sales | 0.90 |
| AJE-5 | Reclassify savings transfer #1022 | Shopify Sales | Savings (or Director's loan) | 2,500.00 |
| AJE-6 | Remove duplicate NC-8841 #1029 | Business Checking (or Vendor receivable) | Shipping & Delivery | 418.60 |
| AJE-7 | Gross up Shopify payouts | Refunds 2,976.75 / Chargebacks & adjustments 221.60 / Merchant fees 2,062.63 | Shopify Sales | 5,260.98 |
| AJE-8 | Reclassify market stall fee | Advertising & Marketing | Ask My Accountant | 120.00 |

## 4. Adjusted P&L summary: August 2026

| | Reported (QBO) | Adjusted |
|---|---:|---:|
| Gross sales | 91,439.92 | 99,657.52 |
| Refunds | | (2,976.75) |
| Chargebacks / adjustments (pending #11) | | (221.60) |
| **Net revenue** | **91,439.92** | **96,459.17** |
| Cost of goods sold (purchases, see #13) | 16,838.70 | 16,838.70 |
| **Gross profit** | **74,601.22** | **79,620.47** |
| Merchant (Shopify) fees | | 2,062.63 |
| Advertising & Marketing | 1,300.00 | 1,420.00 |
| Rent or Lease | 1,850.00 | 1,850.00 |
| Shipping & Delivery | 837.20 | 418.60 |
| Software & Subscriptions | 259.00 | 259.00 |
| Office Supplies | 38.99 | 38.99 |
| Meals | 14.20 | 14.20 |
| Ask My Accountant | 120.00 | 0.00 |
| Uncategorized (pending #8, #9) | 275.83 | 275.83 |
| **Total expenses** | **4,695.22** | **6,339.25** |
| **Net income** | **69,906.00** | **73,281.22** |

**Bridge from reported to adjusted net income:** 69,906.00 + 8,612.89 (missing payout) − 2,257.17 (duplicate payout) − 900.00 (#1011) + 0.90 (keying errors) − 2,500.00 (transfer) + 418.60 (duplicate courier bill) = **73,281.22**

The adjusted figure is before VAT (#12), inventory (#13) and cut-off (#15). Any of these could change the result materially.

