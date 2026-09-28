# Report definitions

### Product margin — which products lose money
Created:   [run date]
Last run:  [run date] (period: 2026-08)
Cadence:   one-off (rerun monthly on request)

Metrics:    net revenue ex VAT = (line price × qty − pro-rata discount − pro-rata partial refund) / 1.19;
            COGS = qty × unit_cost (cogs.csv); gross profit = revenue − COGS; margin = GP / revenue;
            profit per unit = GP / units
Grouping:   product (SKU)
Comparison: unit cost vs ex-VAT price; status LOSS (<0), THIN (<30%), OK, NO COST (SKU missing from cogs.csv)
Period:     calendar month of the orders export
Sources:    Shopify orders export CSV + cogs.csv (no connectors)
Rules:      prices include 19% VAT; exclude voided/cancelled, 'test'-tagged, fully refunded orders;
            shipping and payment fees not included (not in data); never guess a missing unit cost
Script:     `python product_margin_report.py files/orders_export.csv files/cogs.csv`

Revisions:
