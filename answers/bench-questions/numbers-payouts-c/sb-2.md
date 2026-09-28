<!-- small-business / numbers-payouts-c / run 2: skill called by name: month-end-prep; passed -->

The gap is **GBP 18,917.53**. I found no missing money: every card order in Shopify matches a payout line, and refunds and fee rates agree with the orders export. August orders totalled **GBP 113,314.07** and Shopify Payments paid out **GBP 94,396.54** in August. The difference breaks down like this:

| | GBP |
|---|---:|
| Orders placed in August (gross, incl. VAT and shipping) | 113,314.07 |
| Paid through PayPal, so the money went to PayPal, not these payouts (132 orders) | −7,706.80 |
| Paid with gift cards; that cash came in when the cards were sold (48 orders fully, 36 partly) | −4,211.20 |
| Test orders, never real money (4 tagged "test", 4 on the Bogus test gateway) | −912.85 |
| Orders cancelled before the card was charged (7) | −887.45 |
| **Charged to cards through Shopify Payments** | **99,595.77** |
| Shopify processing fees (2.03% overall, the same as June and July) | −2,019.03 |
| Refunds paid in August (1,093.51 on July orders, 1,668.90 on August orders) | −2,762.41 |
| Chargebacks: 3 disputes at 223.95 plus 15.00 fee each | −268.95 |
| Shopify adjustment | +2.35 |
| **August card activity, net** | **94,547.73** |
| 30–31 August sales, paid out 1–2 September | −6,075.32 |
| 29–31 July sales, paid out in August | +5,924.13 |
| **Paid out in August** | **94,396.54** ✓ |

**What that means**
- **GBP 7,706.80 is in PayPal.** This is the biggest item. Check that your PayPal balance was actually moved to the bank. PayPal isn't in these files, so I can't confirm it.
- **GBP 5,050.39 is the real cost of trading:** fees, refunds and chargebacks. None of it looks unusual.
- **GBP 1,800.30 was never a sale:** tests and cancelled orders. Shopify's order total still counts them.
- **GBP 4,211.20 is gift card redemptions.** The cash came in when the cards were sold.
- **The payout timing nets to only GBP 151.19,** because the late-July payouts that landed in August almost cancel out the late-August ones that landed in September.

**Worth acting on**
1. **Three chargebacks are still open:** #32603, #32955 and #33706, totalling GBP 268.95 including the fees. There's no "won" line for any of them yet, so respond in Shopify admin before the deadline. #30226 from June (GBP 138.00) looks lost.
2. **Part of each deposit belongs to HMRC.** About GBP 18,887 of August's order total is VAT.
3. **GBP 4,778.30 of pre-orders was paid but hasn't shipped.** Under your rules that isn't a sale yet, even though the cash has arrived.

**What I couldn't check**
- **Your bank statement.** I've treated "reached the bank" as the payouts Shopify marks as paid. It's worth ticking the 21 August payouts off against the statement.
- **PayPal.**
- **The accounting ledger.** None is connected, so this answers your question but isn't a full close, and I haven't produced the close packet.

If you share the August bank statement and a PayPal activity export, I can match both, or run the full August close once your ledger is connected.
