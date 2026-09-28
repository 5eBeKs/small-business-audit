# Report definitions

Saved by Report Builder. Keep this file with your reports; drop it back in the chat and the report reruns without any questions.

---

### Monthly Shopify sales (bookkeeper numbers)
Created:   [run date]
Last run:  [run date] (period: August 2026)
Cadence:   monthly (run on request; no schedule set)

```
Report name:  Monthly Shopify sales
Cadence:      monthly
Period:       prior calendar month, by order Created-at date (store timezone -0400)
Comparison:   prior month (n/a on first run: export held only August + 3 Jul 31 orders)
Grouping:     product (SKU), week of month, payment method

Metrics:
  Gross product sales  =  sum of Subtotal (pre-discount; ties to line qty x price)   [Shopify export]
  Discounts            =  sum of Discount Amount                                    [Shopify export]
  Net product sales    =  gross product sales - discounts                          [Shopify export]
  Shipping charged     =  sum of Shipping                                           [Shopify export]
  Sales tax collected  =  sum of Taxes (liability, not revenue)                     [Shopify export]
  Total collected      =  sum of Total (= net product + shipping + tax)             [Shopify export]
  Refunds              =  sum of Refunded Amount; split product/ship/tax where full [Shopify export]
  Orders, units, AOV   =  count; sum qty on paid lines; net product sales / orders  [Shopify export]

Sources:      uploaded file: Shopify orders export (CSV)
Notes:        Order-level fields sit on the first line of each order only; never sum
              Total across line rows. Exclude orders outside the month, voided or
              cancelled orders, and "Bogus Gateway (for testing)" orders.
              Sample Votive (MO-SMP-001) is a USD 0 add-on; count it separately.
              Processing fees, shipping cost and COGS are not in this export; report n/a.
              Customer emails are dropped from the raw-data tab.
              Tip: export two months at once next time to get a month-over-month comparison.
```

Revisions:
  (none)
