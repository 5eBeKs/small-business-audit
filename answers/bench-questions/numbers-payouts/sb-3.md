<!-- small-business / numbers-payouts / run 3: skill called by name: month-end-prep; passed -->

I've matched all 60 August orders against the Shopify Payments transactions. The orders export totals **EUR 3,022.62**, and payouts of **EUR 2,448.74** were paid out in August. The whole EUR 573.88 difference is explained to the cent. No money is missing: most of it is timing, some was never real money, and the rest is fees and refunds.

## From sales to money paid out

| | EUR | Running total |
|---|---:|---:|
| Order totals in the orders export (60 orders) | | **3,022.62** |
| #1013 is a **test order** (tagged "test", no card charge) but marked "paid" | −80.90 | 2,941.72 |
| #1021 was **voided** on the same day; the card was never charged | −22.90 | 2,918.82 |
| #1055 was paid through **PayPal**, so the money is in your PayPal balance, not Shopify's | −99.00 | 2,819.82 |
| **Refunds**: #1042 in full (60.50) and #1030 in part (10.00) | −70.50 | 2,749.32 |
| **Chargeback** on #1060: the customer's bank took the money back | −19.30 | 2,730.02 |
| **Card processing fees** on 57 charges (about 2.0%) | −56.59 | 2,673.43 |
| **Chargeback fee** on #1060 | −15.00 | 2,658.43 |
| **In transit at month end**: sales from Aug 30–31, paid out Sep 1 (133.56) and Sep 2 (76.13) | −209.69 | **2,448.74** |

The 2,448.74 is the net of 19 payouts from Aug 3 to Aug 31. One of them is a **negative payout of −60.50 on Aug 26**, which is the #1042 refund. Shopify will have taken that amount out of your bank account, so look for a withdrawal, not a deposit. Every charge matched its order to the cent, and every net amount equals the charge minus its fee.

## What to act on

1. **Delete or archive test order #1013 (EUR 80.90).** It's counted as a real sale, so your August sales figure is overstated by that amount.
2. **Respond to the chargeback on #1060.** EUR 34.30 is out (19.30 order plus the 15.00 fee). If you have proof of delivery, submit it in Shopify under Orders → Chargebacks. Otherwise, accept the loss.
3. **Withdraw the EUR 99.00 PayPal payment for #1055** if you haven't already. It will never appear in a Shopify payout.
4. **Plan for the VAT.** EUR 482.58 of the 3,022.62 is VAT included in your prices, so it's owed to the tax office. The 2,448.74 paid out is gross of VAT, and only about 2,000 of it is income.

## What I couldn't check

- **Your bank statement.** I can confirm what Shopify paid out, but not what arrived in the bank. To check that, I need the August bank statement, or I can read the deposits from your books.
- **Payouts from late July.** The payouts export only includes transactions made in August. Sales from Jul 30–31 that were paid out in early August would have landed in the bank in August but aren't in this file. If your bank shows more than 2,448.74 from Shopify, that's the likely reason.
- **The rest of the month-end close.** There's no bookkeeping system connected, so I haven't checked for uncategorised entries, duplicate payments or missing receipts, and I haven't written a P&L. If you connect QuickBooks, Xero or Zoho Books, or send the P&L and transaction detail as exports, I can finish the August close.
