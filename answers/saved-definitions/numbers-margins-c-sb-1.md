# Report definitions

Saved by Report Builder. Keep this file with your reports. Drop it into the chat next time and the report reruns without any questions.

### Product profit — which products lost money
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   one-off (rerun on request for any month)

```
Report name:  Product profit — which products lost money
Cadence:      one-off, rerunnable by month
Period:       calendar month, by order Created at date
Comparison:   prior months in the same export (Jun, Jul 2026 on first run)
Grouping:     product (SKU)

Metrics:
  Net revenue ex VAT = (line price × qty − order discount spread pro rata by line value − refunds spread by line value) ÷ 1.20   [orders export]
  COGS               = qty × unit_cost   [cogs.csv, SKU matched ignoring case and spaces]
  Profit             = Net revenue ex VAT − COGS;  loss-maker = Profit < 0
  Breakeven cost     = Net revenue ex VAT ÷ units (reported when a SKU has no cost)

Sources:      uploaded files: files/orders_export.csv (Shopify export), files/cogs.csv, files/store_definitions.json
Notes:        Prices include 20% VAT. Rules from store_definitions.json: exclude test orders (tag "test"
              OR payment method "Bogus Gateway (for testing)"); a sale counts only once fulfilled (pre-orders,
              voided and refunded-before-shipping out); shipping excluded from revenue; partial refunds
              amount only, in the order month. Full refunds on shipped orders keep COGS. Free sample
              sachet (GL-SMP-001) shown as a giveaway loss. GL-NEW-001 has no cost on file: show n/a, never estimate.
              Outputs: chat summary, <Month>_product_profit.xlsx, HTML page.
```
