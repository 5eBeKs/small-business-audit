# Report definitions

### Monthly sales summary for the accountant (Shopify)
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   monthly, on request ("how did <month> go", "numbers for my accountant")

Source:     Shopify orders export CSV (files/orders_export.csv). No connector. Shopify is the only revenue source.
Rules:      files/store_definitions.json. VAT-exclusive at 20%. Only shipped orders count, so pre-orders are out.
            Shipping is not revenue. Test orders ('test' tag or Bogus Gateway) are out, and so are cancelled or voided ones.
            Refunds come off by amount only, in the month the order was placed, split between goods and shipping in proportion.
Period:     calendar month, by order Created at date (London time)
Comparison: prior month, with three-month trend
Metrics:    gross product sales, discounts, refunds, net sales (revenue), orders, AOV,
            shipping charged (memo), output VAT (memo), customer receipts incl. VAT
Grouping:   product (discounts and refunds allocated to lines), payment method, discount code, included vs excluded
Build:      python build_monthly_sales_report.py YYYY-MM
            Writes sales_report_YYYY-MM.xlsx. The HTML page is written from its output.

Revisions:
  (none)
