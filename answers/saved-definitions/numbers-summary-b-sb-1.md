# Report definitions

Saved by report-builder. Drop this file back in the chat next time and the report reruns without any questions.

### Monthly Shopify sales
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   monthly, on request (no schedule set)

Report name:  Monthly Shopify sales
Cadence:      monthly
Period:       prior calendar month, by order Created at date (store time, -0400)
Comparison:   prior month (only when the export holds a full prior month; else n/a)
Grouping:     product (SKU), week

Metrics:
  Orders                 =  count of orders in period, excl. voided/cancelled and Bogus Gateway tests  [Shopify export]
  Gross merchandise      =  sum of line items (Subtotal)             [Shopify export]
  Discounts              =  sum of Discount Amount                   [Shopify export]
  Net merchandise        =  gross - discounts                        [Shopify export]
  Shipping charged       =  sum of Shipping                          [Shopify export]
  Sales tax collected    =  sum of Taxes (liability, not revenue)    [Shopify export]
  Total billed           =  sum of Total                             [Shopify export]
  Refunds                =  sum of Refunded Amount                   [Shopify export]
  Billed less refunds    =  total billed - refunds                   [Shopify export]
  Average order value    =  total billed / orders                    [Shopify export]
  Processing fees        =  n/a unless a Shopify Payments payout report is supplied

Sources:      uploaded file: Shopify orders export (CSV). Build script: build_august_report.py
              (run: python build_august_report.py files/orders_export.csv 2026-09)
Notes:        For the owner's bookkeeper. The export mixes in orders from the last day of the prior
              month; exclude them by Created at. Order-level fields sit only on the first line of each
              order. Flag gift-card-paid orders and refund splits the export doesn't break out.

Revisions:
  (none)
