<!-- small-business / numbers-payouts-b / run 1: skill called by name: month-end-prep; passed -->

## The short answer

Your August orders total **USD 4,335.23**. Shopify Payments paid out **USD 3,713.86** in August, across 20 payouts dated Aug 3–31. That's a gap of **USD 621.37**, and I can account for all of it to the cent. About USD 330 of it is not lost money: some of it will arrive in September, and some of it was never card money in the first place.

## Where the USD 621.37 went

| # | Item | USD | Money lost? |
|---|---|---:|---|
| 1 | **Payouts that land in September.** 3 orders from Aug 30–31 (#2052, #2066, #2067) were still "in transit" at month end, due Sep 1–2. This is partly offset by 3 July 31 orders (#1998–#2000) that were paid out on Aug 3. | 181.37 (280.94 − 99.57) | No, just timing |
| 2 | **Card processing fees**: 2.9% + 30¢ on every charge. All 67 charges were billed at exactly that rate, so there were no fee errors. | 136.18 | Yes, a normal cost |
| 3 | **Orders that were never card money:** | 149.60 | See below |
|   | • #2011 and #2044 were paid through the **"Bogus Gateway (for testing)"** | 79.25 | ⚠️ See flag |
|   | • #2008 was **voided/cancelled** on Aug 28 | 50.35 | No, it wasn't a real sale |
|   | • USD 20 of #2051 was paid with a **gift card** (you got that cash when the card was sold) | 20.00 | No |
| 4 | **Dispute (chargeback) on #2027**: the order amount plus a USD 15 dispute fee were taken out on Aug 17. There's no resolution in the data. | 96.51 | Yes, unless you win it |
| 5 | **Refunds**: #2038 was refunded in full (46.06) and #2049 partly (12.00). Shopify keeps the original card fee on refunds. | 58.06 | Yes |
| 6 | Small credit adjustment on #2033 | −0.35 | You gained |
| | **Total** | **621.37** | |

There was also a second dispute, on #2015 (USD 83.66). You **won** it: the money and the USD 15 fee were returned on Aug 26, so it nets to zero. It did make the Aug 14 and Aug 17 payouts look unusually small, though.

## What needs your attention

1. **The two test-gateway orders (#2011, #2044, USD 79.25).** Both are marked *paid* and *fulfilled*, but no money came in through the test gateway. If they were real customers, you shipped product without being paid. If they were tests, delete or archive them so they stop counting as sales.
2. **The #2027 dispute (USD 96.51 on hold).** Check Shopify Admin → Orders → #2027 → Disputes and submit evidence before the deadline. You won the last one.
3. **Watch for September.** The Sep 1 and Sep 2 payouts should come to USD 271.90 in total (126.40 + 145.50). If they don't, let me know.

## Scope

- **Payout timing:** I counted payouts by the date they were paid (Aug 3–31) and orders by the date they were created. Nothing is missing or double-counted: every card charge matches its order.
- **"What we sold" includes tax and shipping:** the USD 4,335.23 includes USD 293.03 of sales tax you collected and USD 250.20 of shipping. Product sales after discounts were **USD 3,792.00**, and that's the revenue figure for your books.
- **Bank not checked:** you only sent the two Shopify files, with no bookkeeping ledger or bank statement. So I haven't checked that these payouts actually reached your bank account.

If you want the full August close (bank match, duplicate scan, missing receipts, P&L summary and close packet), connect your bookkeeping software or send a P&L and transaction export for August.
