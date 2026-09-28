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
