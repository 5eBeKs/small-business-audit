<!-- small-business / numbers-payouts-b / run 2: skill called by name: month-end-prep; passed -->

The gap is USD 621.37, and none of it is money that went missing. It comes from counting different things over different dates. I tied it out to the cent from your two exports.

- **Total of your August orders:** USD 4,335.23 (70 orders)
- **Paid out to you in August:** USD 3,713.86 (20 payouts, Aug 3 – Aug 31)

## How the order total becomes the payout

| Step | Amount (USD) | Running total |
|---|---:|---:|
| August orders, "Total" column | | 4,335.23 |
| **Not real money** | | |
| #2011 and #2044 were paid through "Bogus Gateway (for testing)" | −79.25 | 4,155.98 |
| #2008 was cancelled the same day, so the card was never charged | −50.35 | 4,105.63 |
| #2051: USD 20 was paid with a gift card, which isn't new cash | −20.00 | 4,085.63 |
| **Timing** | | |
| + July 31 orders #1998–#2000, paid out Aug 3 | +99.57 | 4,185.20 |
| − Aug 30–31 orders #2052, #2067, #2066, paid out Sep 1–2 | −280.94 | 3,904.26 |
| **Money actually taken out** | | |
| Card processing fees on 67 orders | −136.18 | 3,768.08 |
| Refunds: #2038 in full, plus USD 12 on #2049 | −58.06 | 3,710.02 |
| Chargeback on #2027, still open (USD 81.51 plus a USD 15 fee) | −96.51 | 3,613.51 |
| Chargeback on #2015: taken Aug 14, won and returned Aug 26 | 0.00 | 3,613.51 |
| Small adjustment on #2033 | +0.35 | 3,613.86 |

That leaves USD 100 still unexplained, which means I mis-ordered a line. Here is the corrected math:

- The three "not real money" lines total USD 149.60, so the start becomes 4,335.23 − 149.60 = **4,185.63**. This is exactly what your card processor charged for August orders.
- Adding July's USD 99.57 and removing the Aug 30–31 orders' USD 280.94 gives **4,004.26**. This matches the charges paid out in August.
- Then: 4,004.26 − 136.18 − 58.06 − 96.51 + 0.35 = **3,713.86**. This matches the payout file exactly.

## Where the USD 621.37 went

| Reason | USD | Share |
|---|---:|---:|
| Timing: 3 orders pay out in September, minus 3 July orders paid in August | 181.37 | 29% |
| Test orders, a cancelled order and a gift card (never card money) | 149.60 | 24% |
| Card processing fees | 136.18 | 22% |
| Open chargeback on #2027 | 96.51 | 16% |
| Refunds | 58.06 | 9% |
| Adjustment | −0.35 | — |

Only fees, refunds and the chargeback (about USD 290) are money you actually lost. The timing difference comes back on your Sep 1–2 payouts.

## What needs you
1. **Respond to the #2027 chargeback in Shopify** (Orders → #2027 → dispute). It's still open. You won #2015 this month and got the fee back as well, so it's worth answering.
2. **Delete test orders #2011 and #2044.** Right now they make your sales look USD 79 higher than they were, in every report that uses the orders data.
3. **Check the +USD 0.35 adjustment on #2033.** It's small and positive, but the file doesn't say why it happened.
4. **Watch the chargebacks.** Two in one month out of about 65 orders is high for a store this size. Both were Discover cards.

A side note on the "Total" column: it includes about USD 293 in sales tax and your shipping charges. Those are passed through the payout, but they aren't product sales, so compare against subtotal when you ask "what did we sell."

I didn't check these payouts against your bank account or books because I only had the two Shopify exports. If you'd like, I can connect your ledger or take a bank statement and run the full August close, including checking the 20 payouts against the bank.
