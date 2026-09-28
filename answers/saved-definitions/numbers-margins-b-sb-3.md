# Report definitions

### Product profitability (which products lose money)
Created:   [run date]
Last run:  [run date]
Cadence:   one-off (can be rerun monthly)

```
Report name:  Product profitability
Cadence:      one-off
Period:       calendar month (first run: August 2026, by order Created at)
Comparison:   none (first run); prior month on rerun
Grouping:     product / SKU

Metrics:
  Net revenue   =  line price x qty, ex sales tax, less order discounts and partial
                   refunds (ex tax), allocated pro rata by line value   [Shopify orders export]
  COGS          =  qty x unit_cost, SKU matched ignoring case and spaces   [cogs.csv]
  Gross profit  =  net revenue - COGS; flag any SKU below zero   [both]
  Gross margin  =  gross profit / net revenue   [both]

Sources:      uploaded files — files/orders_export.csv + files/cogs.csv
Notes:        Owner: prices exclude sales tax. Excluded: orders outside the month,
              voided/cancelled, Bogus Gateway test orders, fully refunded orders.
              Shipping and tax are not product revenue. Payment fees, shipping labels
              and packaging are not in the data, so they are excluded.
              Every SKU on the cost sheet is listed, even with zero sales.
```
