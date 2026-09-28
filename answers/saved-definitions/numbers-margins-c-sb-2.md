# Report definitions

### Monthly product profitability (loss-makers)
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   one-off (rerun on request, e.g. "run the product profitability for September")

Report name:  Monthly product profitability (loss-makers)
Cadence:      one-off, rerunnable
Period:       one calendar month by order date (UK time, +0100)
Comparison:   prior month (the workbook shows the two months before)
Grouping:     product (SKU, normalised: trimmed + upper-case)

Metrics:
  Revenue ex VAT  =  (line price x qty, less order discount pro-rata, less refund pro-rata) / 1.20   [Shopify orders export]
  COGS            =  units shipped x unit cost   [cogs.csv]
  Gross profit    =  revenue ex VAT - COGS; a product "lost money" when this is below zero
  Margin          =  gross profit / revenue ex VAT

Sources:      uploaded files: Shopify orders_export.csv, cogs.csv, store_definitions.json
Notes:        Rules from store_definitions.json: leave out test orders (tag 'test' or Bogus Gateway); a sale
              counts only once shipped (pre-orders/unfulfilled left out); leave out voided/cancelled; remove 20% VAT;
              keep shipping out of revenue; partial refunds take off the amount only, split pro-rata between
              goods and shipping, and belong to the order month. COGS still counted on refunded orders (no restock
              data). Checked: doesn't change the loss list. SKU with no cost in cogs.csv → profit "n/a", with
              its break-even unit cost shown.
              Aug 2026 result: Sample Sachet, Summer Tin (clearance), Old Label Serum (clearance) lost money;
              GL-NEW-001 Peptide Serum had no cost on file.
