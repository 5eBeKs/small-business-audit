# Report definitions

### Monthly Shopify sales for the accountant
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   monthly, run on request (no schedule set)

```
Report name:  Monthly Shopify sales for the accountant
Cadence:      monthly, on request
Period:       prior calendar month, by paid date
Comparison:   prior month (n/a when the export covers one month only)
Grouping:     product; week

Metrics:
  Orders               =  count of orders, excl. voided/cancelled and "test"-tagged   [Shopify orders CSV]
  Gross product sales  =  sum of Subtotal (line items, VAT incl., pre-discount)      [Shopify orders CSV]
  Discounts            =  sum of Discount Amount                                      [Shopify orders CSV]
  Shipping             =  sum of Shipping                                             [Shopify orders CSV]
  Total order value    =  sum of Total (= subtotal - discounts + shipping)            [Shopify orders CSV]
  Refunds              =  sum of Refunded Amount                                      [Shopify orders CSV]
  Net collected        =  total order value - refunds                                 [Shopify orders CSV]
  Net VAT              =  sum of Taxes - 19/119 x refunds                             [Shopify orders CSV]
  Net sales excl. VAT  =  net collected - net VAT                                     [Shopify orders CSV]
  AOV, units, sales by product, sales by week (per-day normalized)                    [Shopify orders CSV]
  Processor fees       =  n/a unless a payout report is supplied                      [Shopify Payments payouts]

Sources:      uploaded file — Shopify orders export (orders_export.csv)
Notes:        Currency EUR; prices include 19% VAT.
              Voided orders and orders tagged "test" are excluded and listed.
              Aug 2026: #1013 (EUR 80.90, tagged test but paid) excluded pending owner confirmation.
              Refund dates are not in the orders export; refunds assumed in-period.
              Include the prior month's export next time to get the vs-prior-month comparison.
```
