# Report definitions

### Monthly Shopify sales summary (for the accountant)
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   monthly, on request (owner drops the month's Shopify orders export)

```
Report name:  Monthly Shopify sales summary
Cadence:      monthly, on request
Period:       prior calendar month (by Paid at date)
Comparison:   prior month — n/a until a prior month's export is supplied
Grouping:     product (SKU), week, payment method

Metrics:
  Orders                 =  count of orders, excluding voided          [uploaded Shopify CSV]
  Gross sales incl. VAT  =  sum of order Total = items + shipping − discounts   [CSV]
  Refunds                =  sum of Refunded Amount                     [CSV]
  Net sales incl. VAT    =  gross − refunds                            [CSV]
  Net VAT                =  sum of Taxes − refunds × 19/119            [CSV]
  Net revenue excl. VAT  =  net sales incl. VAT − net VAT              [CSV]
  AOV, units, sales by SKU, sales by week, sales by payment method     [CSV]
  Processing fees        =  n/a — not in the orders export

Sources:      uploaded file — Shopify orders export (orders_export.csv), EUR, prices VAT-inclusive at 19%
Notes:        Voided orders excluded. Orders tagged "test" are counted but flagged for confirmation.
              Refund dates are not in the export; flag them for the accountant.
              Rebuild script: build_monthly_sales_report.py in this folder
              (python build_monthly_sales_report.py <csv> "<Month YYYY>").
```

Revisions:
  (none)
