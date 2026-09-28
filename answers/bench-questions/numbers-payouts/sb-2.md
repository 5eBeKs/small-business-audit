<!-- small-business / numbers-payouts / run 2: skill called by name: month-end-prep; passed -->

I've traced the whole gap and every euro is accounted for. No money went missing: the difference comes from money that never came through Shopify Payments, fees and refunds taken out, and payouts that reached the bank in September.

## August: from orders to payouts

| | EUR |
|---|---:|
| **Order totals in the orders export (60 orders)** | **3,022.62** |
| Test order #1013, tagged "test", never charged | −80.90 |
| Order #1021 cancelled and voided, never charged | −22.90 |
| Order #1055 paid by PayPal, so it went to PayPal, not Shopify | −99.00 |
| **Card payments Shopify collected (57)** | **2,819.82** |
| Refunds: #1042 in full (60.50) and #1030 in part (10.00) | −70.50 |
| Chargeback on #1060: the sale taken back plus a 15.00 dispute fee | −34.30 |
| Card processing fees, about 2% | −56.59 |
| Sales from 30–31 Aug, paid out on 1–2 Sep | −209.69 |
| **Paid out to your bank in August (19 payouts)** | **2,448.74** |

These totals tie exactly to the payout export, and every card payment matches its order to the cent.

## What stands out

1. **The PayPal order (EUR 99.00)** is sitting in your PayPal account, not in a Shopify payout. Check it reached your bank from PayPal.
2. **The chargeback on #1060** cost EUR 34.30, but the orders export still shows the order as "paid." That means your sales reports are overstated for it. Consider responding to the dispute; the order was only EUR 19.30, so the 15.00 fee is most of the loss.
3. **Test order #1013 (EUR 80.90)** is marked "paid," so it inflates your sales numbers. Please confirm in Shopify that it really was a test. If it was a real customer, those are the only euros I can't trace.
4. **The 26 Aug payout was negative (−60.50).** That was the full refund on #1042. Your bank statement should show it as a withdrawal, not a deposit, so don't count it as missing income.
5. **Early-August deposits may include July sales.** The payout export only starts at 1 Aug. Payouts for sales from the last days of July would show up in your bank in early August but aren't in this file. If you compare this file to your bank, expect a few extra deposits at the start of the month.
6. **Not a leak, but worth knowing:** EUR 482.58 of the order totals is VAT. It's in your deposits, but it's owed to the tax office, so it isn't income you can spend.

## What I couldn't check

I don't have your bank statement or your accounts, so I haven't confirmed that the 19 payouts actually arrived. The figure above is what Shopify says it paid out. To finish that check and do the rest of the month-end close, I'd need:
- your **August bank statement**, so I can match each payout by amount and date (within 2 days)
- your **PayPal activity for August**, to find the EUR 99.00
- the **payout export from late July**, to explain any extra early-August deposits

With your P&L report and transaction list from your accounting software, I can also do the rest of the close: flag uncategorized entries, check for duplicate charges and missing receipts, and write the month summary.
