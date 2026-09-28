<!-- small-business / numbers-summary-b / run 3: skill called by name: report-builder; passed -->

## Shopify sales for August 2026 (Aug 1–31)

August brought in **USD 3,644.00 in net sales from 67 orders**. I can't say yet whether that's up or down: the export only has 3 orders from July, so there's nothing to compare against.

**Net sales:** USD 3,644.00 (no July baseline)
**Orders:** 67, averaging USD 55.10 in merchandise after discounts
**Total collected:** USD 4,147.57, including USD 222.40 shipping and USD 281.17 sales tax, after refunds

### Numbers for your bookkeeper

| Line | August |
|---|---|
| Gross sales | USD 3,702.00 |
| Discounts (SUMMER5, 2 orders) | (USD 10.00) |
| Returns | (USD 48.00) |
| **Net sales** | **USD 3,644.00** |
| Shipping | USD 222.40 |
| Sales tax (you owe this, it's not income) | USD 281.17 |
| **Total sales** | **USD 4,147.57** |

The total matches the order totals minus refunds exactly, and the product rows add up to gross sales.

### What stands out

- **Reed Diffuser makes up a third of your sales:** USD 1,248 from 39 units, or 34% of gross. No other product is above 18%.
- **6 orders in the file (USD 229.17) aren't August sales, so I left them out:** 3 from July 31, 1 voided order (#2008), and 2 test orders (#2011 and #2044, USD 79.25) run through Shopify's test payment option. Anyone who just adds up the raw file will get a number that's too high.
- **USD 58.06 went back to customers:** #2038 was refunded in full and #2049 got a USD 12.00 partial refund.

### Worth checking before this goes to the bookkeeper

- **#2049's USD 12.00 refund:** the export doesn't say whether it was for product, shipping or tax. I counted it as a product return. If part of it was tax, the tax figure changes slightly.
- **#2051 (USD 120.12) was paid partly with a gift card.** That part won't show up in your Shopify Payments payouts, so it won't match your bank deposits. The export doesn't show how the payment was split.
- **Not in the file:** Shopify Payments fees, payout amounts and cost of goods. So this covers sales, not profit.

### Files in your folder

- `Shopify_Sales_2026-08.xlsx`: tabs for Summary, By product, By week, Flagged & excluded, Included orders and Raw data.
- `Shopify_Sales_2026-08.html`: a one-page version of the report to open in a browser.

I couldn't save the report setup to the skill's own folder because it's protected, so I put it in `report-definitions.md` in your folder instead. Keep that file with your reports. Next month, drop in the September export and I'll run the same report without asking you anything.

**Next step:** export July's orders from Shopify and I'll add the month-over-month comparison. If you want the fees and payouts matched against your books too, `/close-month` does that.

<!-- saved for the owner: report-definitions.md -->

# Report definitions

### Monthly Shopify sales (bookkeeper numbers)
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   monthly

```
Report name:  Monthly Shopify sales (bookkeeper numbers)
Cadence:      monthly
Period:       prior calendar month, by order created date (store time, -0400)
Comparison:   prior month (n/a on first run: export held only Jul 31 orders)
Grouping:     product; week within month

Metrics:
  Gross sales     =  sum of line price x qty, included orders            [Shopify orders CSV]
  Discounts       =  sum of Discount Amount                              [Shopify orders CSV]
  Returns         =  product portion of Refunded Amount                  [Shopify orders CSV]
  Net sales       =  gross - discounts - returns
  Shipping        =  shipping charged - shipping refunded
  Sales tax       =  taxes charged - taxes refunded (liability)
  Total sales     =  net + shipping + tax; must tie to sum(Total) - sum(Refunded Amount)
  Orders, AOV (merch after discounts / orders), paid units, refunds paid out

Sources:      uploaded file: Shopify Orders export CSV (files/orders_export.csv)
Notes:        Exclude: orders outside the month, voided/cancelled, Bogus Gateway test orders.
              Full refunds split by the order's own product/shipping/tax. Partial refunds
              treated as product returns and flagged (export doesn't allocate them).
              Flag gift-card tender (not in Shopify Payments payouts).
```

Revisions:
  (none)


<!-- saved for the owner: Shopify_Sales_2026-08.html -->

 Shopify Sales — August 2026 
 SB Shopify Sales — August 2026 Aug 1–31, 2026 · orders by created date · built from orders_export.csv on [run date], 2026 
 What stands out 
 Reed Diffuser is a third of the business: USD 1,248.00 on 39 units, 34% of gross sales. No other product tops 18%. 
 6 orders (USD 229.17) in the export aren't August sales and are left out: 3 from July 31, 1 voided, and 2 test-gateway orders (USD 79.25). A bookkeeper summing the raw file would overstate the month. 
 USD 281.17 of the money collected is sales tax , a liability to remit, not income. USD 58.06 was refunded to customers across 2 orders. 
 USD 3,644.00 Net sales After USD 10.00 discounts and USD 48.00 returns. No July baseline to compare. 
 67 Orders Average order USD 55.10 in merchandise after discounts. 
 USD 4,147.57 Total collected Net sales + USD 222.40 shipping + USD 281.17 tax, less refunds. 
 Bookkeeper breakdown Line August 2026 Gross sales USD 3,702.00 Discounts (USD 10.00) Returns (USD 48.00) Net sales USD 3,644.00 Shipping USD 222.40 Sales tax (liability) USD 281.17 Total sales USD 4,147.57 
 By product Product Units Gross sales Share Reed Diffuser 39 USD 1,248.00 34% Cedar Candle 8oz 28 USD 672.00 18% Fig Candle 8oz 22 USD 528.00 14% Travel Tin Trio 24 USD 468.00 13% Match Cloche 34 USD 408.00 11% Wick Trimmer 27 USD 378.00 10% Sample Votive 9 USD 0.00 0% Gross before discounts and returns; rows sum to USD 3,702.00. Sample Votive is a free add-in. 
 By week Week Orders Gross sales Aug 1–7 13 USD 717.50 Aug 8–14 20 USD 879.50 Aug 15–21 14 USD 852.50 Aug 22–28 14 USD 853.50 Aug 29–31 3 days 6 USD 399.00 
 Flagged & excluded orders Order Date Type Amount Treatment #2020 2026-08-06 Discount USD 5.00 Code SUMMER5. Shown in the Discounts line. #2033 2026-08-08 Discount USD 5.00 Code SUMMER5. Shown in the Discounts line. #2038 2026-08-05 Full refund USD 46.06 Refunded in full (USD 36.00 product, 6.95 shipping, 3.11 tax). Order counted in gross, reversed in returns. #2049 2026-08-24 Partial refund USD 12.00 Export doesn't say what was refunded. Treated as a product return (pre-tax). Check the refund in Shopify admin; if any of it was tax, the tax figure moves. #2051 2026-08-19 Gift card tender USD 120.12 Paid partly by gift card. Counted as a sale (redemption). The gift-card portion won't appear in Shopify Payments payouts; the split isn't in the export. #1998 2026-07-31 Excluded USD 33.19 Created 2026-07-31 — outside 2026-08 #1999 2026-07-31 Excluded USD 33.19 Created 2026-07-31 — outside 2026-08 #2000 2026-07-31 Excluded USD 33.19 Created 2026-07-31 — outside 2026-08 #2008 2026-08-28 Excluded USD 50.35 Voided / cancelled — payment never captured #2011 2026-08-11 Excluded USD 20.32 Test order (Bogus Gateway) — not a real sale #2044 2026-08-15 Excluded USD 58.93 Test order (Bogus Gateway) — not a real sale 
 Not available this run: July 2026 orders (no month-over-month comparison), Shopify Payments fees and payouts, cost of goods. Generated by Report Builder — Small Business 
 
