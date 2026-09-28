<!-- small-business / numbers-payouts-c / run 1: skill called by name: month-end-prep; passed -->

Of the gap between what you sold in August and what reached the bank, only about **GBP 5,050 was actually lost**, to card fees, refunds and chargebacks. The rest of the difference is timing, money still sitting in PayPal, or sales that were never cash in August.

**How I measured it:** "Sold" is the total of every order created in August (GBP 113,314.07, 1,640 orders). "Reached the bank" is the 21 Shopify Payments payouts dated in August (GBP 94,396.54). The gap is **GBP 18,917.53**, and the steps below account for all of it to the penny.

| | GBP |
|---|---:|
| **Orders created in August** | **113,314.07** |
| Test orders (4 tagged "test", 4 through the test gateway) | −912.85 |
| Voided orders, where the payment was never taken (6) | −887.45 |
| Paid by PayPal (132 orders), which goes to your PayPal balance and not this payout | −7,706.80 |
| Paid by gift card (GBP 3,586.00 full plus GBP 625.20 part-paid). That cash came in when the cards were sold | −4,211.20 |
| **Card charges through Shopify Payments** | **99,595.77** |
| Processing fees (2.03% of charges, in line with June and July) | −2,019.03 |
| Refunds paid out: GBP 1,668.90 on August orders and GBP 1,093.51 on July orders | −2,762.41 |
| Chargebacks (#32603, #32955, #33706) plus a GBP 15 fee on each | −268.95 |
| Shopify adjustment | +2.35 |
| August sales paid out on 1–2 Sept, still in transit | −6,075.32 |
| Late-July sales paid out in August | +5,924.13 |
| **Payouts in August** | **94,396.54** |

**What to do about it:**
1. **PayPal (GBP 7,706.80) is the biggest piece.** It's probably fine, but these files can't show it. Check that your PayPal balance was moved to the bank.
2. **Three chargebacks are still open (GBP 223.95 plus GBP 45 in fees).** Two July chargebacks were won and the money came back, so these are worth fighting. June's #30226 (GBP 123) was lost.
3. **Timing mostly evens out.** GBP 6,075.32 lands in September and GBP 5,924.13 came in from July. Net effect on August: −GBP 151.19.
4. **Pre-orders:** 70 pre-orders (GBP 4,778.30) were charged and paid out in August but haven't shipped. Your rules only count a sale once it ships, so that is cash received ahead of the sale, not revenue yet.

**What August revenue actually is:** The cash that reached you includes about GBP 17,800 of VAT, which is owed to HMRC. Your rules also leave out shipping, unshipped orders and test orders. On that basis August revenue is about **GBP 85,100** after refunds (roughly GBP 86,500 before them). That's up from about GBP 80,400 in July. I took out VAT at 20%, the rate in your settings. The refund part is approximate because the refund amounts don't say whether they include shipping.

**What I didn't check:** No accounting software or bank statement was provided. "Reached the bank" here means Shopify's payout records, not your statement. So I haven't matched payouts to actual deposits, scanned for duplicate transactions or checked receipts. With your August bank statement and PayPal activity export, I can match each payout to its deposit and close out the PayPal question. After that I can build the full close packet if you want it.
