<!-- small-business / numbers-payouts-c / run 3: skill called by name: month-end-prep; passed -->

I've traced the whole August gap and nothing is missing. Every order ties to its Shopify Payments charge, every refund ties to its order, and the bridge below balances to the penny. The gap is money that goes somewhere other than your Shopify Payments payouts, plus fees, refunds and chargebacks.

## August: orders placed vs Shopify Payments payouts

| | GBP |
|---|---:|
| **Order value, all 1,640 orders placed in August** | **113,314.07** |
| − Test orders (4 tagged "test", 4 paid through the testing gateway, so never real money) | −912.85 |
| − Orders cancelled before the card was charged (6) | −887.45 |
| − Paid by PayPal (132 orders); this goes to your PayPal account, not these payouts | −7,706.80 |
| − Paid by gift card (48 orders fully, 36 in part) | −4,211.20 |
| **= Card charges through Shopify Payments** | **99,595.77** |
| − Charged 30–31 Aug, paid out 1 Sep ("in transit") | −6,276.05 |
| + Charged late July, paid out in August | +6,337.80 |
| − Card processing fees | −2,017.63 |
| − Refunds returned to cards (GBP 1,380.64 of it is for July orders) | −2,976.75 |
| − Chargebacks (3) plus GBP 15 fee each | −268.95 |
| + Shopify adjustment | +2.35 |
| **= August payouts (net)** | **94,396.54** |

## Where the GBP 18,917.53 went

- **GBP 7,706.80 sits in PayPal, not lost.** The payout file only covers Shopify Payments. Check whether you moved the PayPal balance to the bank. I can't see it from these files.
- **GBP 4,211.20 was paid with gift cards.** That money arrived when each card was bought, or never if you gave cards away as promotions or store credit. No gift card purchases appear in this export, so it's worth checking how they were issued.
- **GBP 5,263.33 actually left the business:** fees 2,017.63, refunds 2,976.75, chargebacks and their fees 268.95.
- **GBP 1,800.30 were never real sales:** test and cancelled orders. Test orders only get left out of sales when they carry the "test" tag or use the test gateway, and these all do.
- **Timing roughly cancels out.** About GBP 6.3k slips from each month into the next, so the net effect in August is +GBP 61.75.

This isn't new to August. Order value was higher than payouts by GBP 16,242 in July and GBP 20,981 in June. June's figure is inflated because the late-May charges paid out in June aren't in the data.

## Things to act on

1. **Three August chargebacks are still open:** #32603 (GBP 41.95), #32955 (GBP 116.00) and #33706 (GBP 66.00). You won both disputes you contested in June and July, so these are worth answering. The June chargeback on #30226 (GBP 123) was never won back.
2. **70 pre-orders worth GBP 4,778.30 were charged in August but haven't shipped.** Under your rule that a sale counts only once it ships, that's cash you've collected ahead of the sale. You'll owe the goods or a refund.
3. **On your own sales rules, August sales were GBP 85,116.** That leaves out VAT, shipping, tests, cancellations, unshipped orders and refunds on August orders. It's up 7% from July (GBP 79,434), so the growth is real.

**What this doesn't cover:** I compared orders to Shopify's payout records. I didn't check the payouts against a bank statement or your bookkeeping, because neither is in the folder. I also haven't reviewed PayPal. For a full August close (bank match, duplicates, receipts, P&L), send your ledger's P&L and transaction exports, the August bank statement, and a PayPal statement with the fee column.
