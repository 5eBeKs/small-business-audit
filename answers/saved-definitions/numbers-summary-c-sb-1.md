# Report definitions

### Monthly Shopify sales report (for accountant)
Created:   [run date]
Last run:  [run date] (period: August 2026)
Cadence:   monthly (run on request; no schedule set)

```
Report name:  Monthly Shopify sales report
Cadence:      monthly
Period:       prior calendar month (order created date, UK time)
Comparison:   prior month, plus the month before for a 3-month view
Grouping:     product (plus daily, discount code, payment method tabs)

Metrics:
  Gross sales     =  sum of Subtotal (pre-discount) / 1.20                  [Shopify export]
  Discounts       =  sum of Discount Amount / 1.20                          [Shopify export]
  Refunds         =  refunded amount / 1.20; full refunds remove goods only [Shopify export]
  Net sales       =  gross - discounts - refunds (ex VAT, ex shipping)      [Shopify export]
  Orders shipped  =  count of counted orders                                [Shopify export]
  AOV             =  net sales / orders shipped                             [Shopify export]
  Memo lines      =  shipping charged ex VAT, VAT collected (pro rata on refunds), cash taken

Sources:      uploaded file — files/orders_export.csv (+ files/store_definitions.json)
Notes:        Rules from store_definitions.json: test orders excluded (tag 'test' or Bogus Gateway);
              sale counts only when fulfilled (pre-orders / unshipped excluded); ex VAT at 20%;
              customer shipping excluded from revenue; partial refunds deduct amount only;
              refunds attributed to order month. Product rows allocate discounts/refunds pro rata
              to line price and must tie to net sales.
Rerun:        python build_report.py . <Month>_Sales_Report.xlsx YYYY-MM
```

Revisions:
