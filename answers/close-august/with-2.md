<!-- close-august / with the plugin / run 2: found 12 of 12 -->

I've closed August as far as the P&L summary. **QuickBooks shows GBP 69,906 net profit, but that figure is wrong.** If you fix the flags below as I recommend, it comes to **GBP 73,281**. I haven't changed anything in QuickBooks.

I assumed the currency is GBP, based on the Shopify export and the "Ltd".

## What needs attention (19 items, all open)

**Shopify payouts vs QuickBooks deposits.** Shopify paid out GBP 94,396.54 in 21 payouts; QuickBooks has GBP 91,439.92 booked as sales. 16 payouts match exactly, and a 17th (6 Aug) is out by GBP 0.30, which is too small to flag. The rest:

| # | Item | Effect on revenue | Fix |
|---|---|---|---|
| 1 | Payout PO-20260810 (GBP 8,612.89) has no deposit in QuickBooks | understated by 8,612.89 | Record it |
| 2 | Deposit #1017 on 27 Aug repeats payout PO-20260825, already booked as #1016 | overstated by 2,257.17 | Check the bank, then void #1017 |
| 3 | #1022 "Transfer from savings" is coded to Shopify Sales | overstated by 2,500.00 | Recode it to the savings/transfer account |
| 4 | #1011 (18 Aug) is booked at 3,222.88; Shopify paid 2,322.88 | overstated by 900.00 | Correct the amount |
| 5 | #1008 (13 Aug) is booked at 3,768.25; Shopify paid 3,768.85 | understated by 0.60 | Correct the amount |

**Duplicate:**
6. Northbound Couriers invoice NC-8841 (GBP 418.60) was paid twice, as #1028 on 12 Aug and #1029 on 14 Aug. If both payments left the bank, ask Northbound for a refund or credit.

**Uncategorised:**
7. #1038 "Card payment", GBP 212.35: no account, payee or memo.
8. #1037 Market stall fee, GBP 120 ("Summer fair"): coded to Ask My Accountant. Advertising & Marketing looks like the right account.
9. #1036 Amazon, GBP 63.48: Uncategorized Expense, no memo.

**Missing receipts** (expenses over GBP 25 with nothing attached in QuickBooks), GBP 1,734.82 in total:
10–15. Meta Ads GBP 940, Photo Studio North GBP 360, Card payment GBP 212.35, Market stall GBP 120, Amazon GBP 63.48 and Office Depot GBP 38.99.

**Questions for you:**
16. Did the summer fair stall take any money outside Shopify? Nothing is recorded.
17. Sales are booked at the net payout amount, so GBP 2,063 of Shopify fees and GBP 2,977 of refunds never show on the P&L. Payout timing also shifts some July sales into August, and some August sales into September.
18. Cost of goods is simply the stock bought in August. There's no stock count, so the margin isn't the real margin.
19. The books have no payroll, VAT or bank-charge lines. Is that expected?

## P&L summary

| | As booked | Corrected* |
|---|---|---|
| Revenue (net payouts) | GBP 91,439.92 | GBP 94,396.54 |
| Cost of goods | GBP 16,838.70 | GBP 16,838.70 |
| Gross margin | 81.6% | 82.2% |
| Operating expenses | GBP 4,695.22 | GBP 4,276.62 |
| **Net income** | **GBP 69,906.00** | **GBP 73,281.22** |

*If items 1–6 are resolved as recommended.

- **Revenue:** before fees and refunds, customers paid GBP 99,658 in August. Refunds took 3% of that.
- **Margin:** 82% looks strong, but it reflects what you bought in August, not the cost of what you sold.
- **Expenses:** these are small, mostly rent (GBP 1,850) and advertising (GBP 1,300).
- **No month-over-month comparison:** I only had August's data.

**For September, watch:**
- Matching every payout to the bank, since three of August's errors were typing mistakes.
- A stock count.
- The missing receipts.

## Skipped
The full month-end process would go on to refresh your cash forecast and send the packet to your accountant. I didn't do either: you asked me to stop at the P&L summary, and a forecast built on books with these open flags would be off. Once the flags are fixed, I can run the 30/60/90-day cash forecast from the corrected books if you want it.

## Files
In `<local path>`:
- `close-packet-2026-08.xlsx`: the P&L (as booked, adjustments and corrected), the payout-by-payout reconciliation, and all 19 action items
- `close-packet-2026-08-summary.pdf`: a one-page summary
- `close-2026-08.html`: a visual page with the same content
