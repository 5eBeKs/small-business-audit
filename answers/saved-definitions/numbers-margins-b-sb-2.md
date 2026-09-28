# Report definitions

### Product profitability (which products lose money)
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   one-off (rerunnable monthly on request)

```
Report name:  Product profitability
Cadence:      one-off; rerun on request for any month
Period:       calendar month, by order Created at (store-local time)
Comparison:   none (first run); prior month once a second month is run
Grouping:     product (SKU)

Metrics:
  Net revenue   =  qty x line price, less pro-rata share of order discount
                   and partial refund; excl. tax and shipping   [orders_export.csv]
  COGS          =  qty x unit_cost                               [cogs.csv]
  Gross profit  =  net revenue - COGS                            [both]
  Margin        =  gross profit / net revenue                    [both]
  Profit / unit =  gross profit / units                          [both]

Sources:      uploaded files — Shopify orders export + cogs.csv (in files/)
Notes:        Owner: prices exclude sales tax.
              Exclude: orders outside the month, voided/cancelled, fully
              refunded, "Bogus Gateway (for testing)" payments.
              Match SKUs trimmed and case-insensitive (cost sheet has a
              "mo-cnd-001 " entry). Every cost-sheet SKU gets a row, even at zero.
              Processing fees, shipping cost, packaging not in data — margins are gross.
              Script: product_margin.py in this folder
                (python product_margin.py files <output.xlsx>; month is set in the script).
```

Revisions:
  (none)
