<!-- small-business / numbers-margins / run 1: skill called by name: report-builder; passed -->

## Product margin: August 2026

**The Steel Strainer is the only product that loses money.** It sells for EUR 6.50, which is EUR 5.46 once you take out the 19% VAT. It costs you EUR 7.10, so you lose about EUR 1.69 on every one you sell.

**Products losing money:** 1 (Steel Strainer), EUR (33.85) in August on 20 units
**Gross margin on products with a known cost:** 45.9%, which is EUR 745.71 profit on EUR 1,623.71 of sales before VAT
**Sales with no cost on file:** EUR 642.18 (28% of product sales). This is all the Gift Set, so I can't tell whether it makes money.

### What stands out

- **Steel Strainer (STR-STL-001).** It doesn't cover its cost even before discounts. To break even the price needs to be at least EUR 8.45 including VAT. 11 of the 13 orders with a strainer also had other items, so it's mostly an add-on. You could keep it as a deliberate loss-leader, raise the price, or find a cheaper supplier.
- **Gift Set (SET-GFT-001) isn't in cogs.csv.** It's your second-biggest product by sales, but I didn't guess a cost for it. It makes money only if it costs you less than EUR 40.14 per set. That's what it actually brought in per unit after discounts and one partial refund, before VAT.
- **All other products make 44–62% gross margin.** Black Tea earns the most in total (EUR 152.46). Glass Teapot has the lowest margin of the rest at 44%, but it made the most profit in euros (EUR 240.76).

### Worth a look

- **Add the Gift Set's cost to cogs.csv and rerun.** That's the one number that could change the answer.

### How I counted
- **Discounts and refunds:** sales are after WELCOME10 discounts and partial refunds, with VAT taken out.
- **Orders left out:** #1013 (tagged "test"), #1021 (voided) and #1042 (fully refunded).
- **Not included:** shipping costs, payment fees and packaging, because the export doesn't have them. Including them would only push margins lower. I found no problems in the source files.
- **Tie-out:** product sales match order totals minus shipping and refunds.

I didn't stop to confirm these rules with you because your question was clear. If you want any of them handled differently, tell me and I'll rerun.

### Files
- **`product_margin_2026-08.html`**: the report page.
- **`product_margin_2026-08.xlsx`**: the workbook, with a summary tab, margin by product, line-by-line detail, excluded orders and the raw data.
- **`product_margin_report.py`**: the script that builds both. Run it on next month's exports to get the same report.

The report ran. I couldn't save the definition to the report-builder skill folder because the edit needed a permission that wasn't granted. I saved it to `report-definitions.md` in this folder instead. Keep that file with your reports and bring it back next time, and I'll rerun this without asking you anything.

**Next step:** add the Gift Set's cost and I'll rerun this. If you want the full picture around these numbers, I can also run `growth-pulse` to see which products are driving sales.

<!-- saved for the owner: product_margin_2026-08.html -->

 Product margin — 2026-08 
 PM Product margin — which products lose money 
 Shopify orders, 2026-08 · prices ex 19% VAT · Generated [run date] 
 What stands out Steel Strainer sells for EUR 6.50 incl VAT = EUR 5.46 ex VAT, against a unit cost of EUR 7.10. That is EUR (1.69) on every unit; 20 units in 2026-08 = EUR (33.85). Break-even shelf price: EUR 8.45 incl VAT. Gift Set (SET-GFT-001) has no unit cost in cogs.csv — EUR 642.18 ex VAT, 28% of product revenue, is unverified. It stays profitable only if its cost is below EUR 40.14 per unit. Everything else earns 44–62% gross margin. Costed products made EUR 745.71 gross profit on EUR 1,623.71 ex VAT (45.9%). 
 1 Product losing money 
 Steel Strainer: EUR (33.85) in 2026-08. 
 45.9% Gross margin, costed products 
 EUR 746 profit on EUR 1,624 ex VAT. 
 EUR 642 Revenue with no cost on file 
 Gift Set: 28% of product revenue, margin unknown. 
 Margin by product 
 Product Status Units Price ex VAT Unit cost 
 Profit / unit Revenue ex VAT Gross profit Margin 
 Steel Strainer STR-STL-001 Loses money 20 EUR 5.46 EUR 7.10 EUR (1.69) EUR 108.15 EUR (33.85) -31.3% Gift Set SET-GFT-001 No cost on file 16 EUR 41.18 n/a n/a EUR 642.18 n/a n/a Matcha 30g TEA-MAT-030 Profitable 8 EUR 20.17 EUR 9.70 EUR 10.47 EUR 161.34 EUR 83.74 51.9% Green Tea 100g TEA-GRN-100 Profitable 13 EUR 10.84 EUR 4.10 EUR 6.57 EUR 138.76 EUR 85.46 61.6% Ceramic Cup CUP-CER-001 Profitable 14 EUR 15.13 EUR 7.50 EUR 7.52 EUR 210.25 EUR 105.25 50.1% Oolong 50g TEA-OOL-050 Profitable 16 EUR 13.45 EUR 6.20 EUR 6.99 EUR 211.09 EUR 111.89 53.0% Black Tea 100g TEA-BLK-100 Profitable 26 EUR 9.66 EUR 3.80 EUR 5.86 EUR 251.26 EUR 152.46 60.7% Glass Teapot 600ml POT-GLS-600 Profitable 19 EUR 28.57 EUR 15.90 EUR 12.67 EUR 542.86 EUR 240.76 44.4% 
 All products (EUR 2,265.90 ex VAT) · costed products only for profit 
 EUR 1,623.71 EUR 745.71 45.9% 
 How this was counted 
 Revenue is the line price after WELCOME10 discounts and partial refunds (allocated by line value), divided by 1.19 to remove VAT. Profit per unit uses actual revenue, so it sits slightly below shelf price minus cost where discounts applied. 
 Left out: #1013 (tagged 'test', EUR 80.90); #1021 (voided / cancelled, EUR 18.00); #1042 (fully refunded, EUR 60.50). Product revenue ties to order totals minus shipping and refunds. 
 Not included: shipping (EUR 151.90 collected incl VAT; shipping cost not in the data), payment fees, packaging, returns handling. These only push margins lower. 
 Not available this run: unit cost for SET-GFT-001; shipping costs; payment fees. Source: orders_export.csv (Shopify export), cogs.csv. Pulled [run date]. · Generated by Report Builder — Small Business 
 

<!-- saved for the owner: report-definitions.md -->

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

