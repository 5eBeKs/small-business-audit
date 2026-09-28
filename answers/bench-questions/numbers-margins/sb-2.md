<!-- small-business / numbers-margins / run 2: skill called by name: report-builder; passed -->

## Product profitability, August 2026

**The Steel Strainer is the only product I can confirm loses money. The Gift Set is your biggest seller, but I can't tell whether it makes money because it isn't in cogs.csv.**

**Losing money:** 1 product, the Steel Strainer. It lost EUR 33.85 in August on 20 units.
**Gross margin on the 7 products that have a cost:** EUR 745.71, which is 45.9% of EUR 1,623.71 net revenue (VAT removed).
**Revenue with no cost to check against:** EUR 642.18. That's 28% of net merchandise revenue, all from the Gift Set.

### What stands out

- **The Steel Strainer is priced below its cost.** It sells for EUR 6.50 including VAT, which is EUR 5.46 after VAT. It costs you EUR 7.10, so you lose EUR 1.64 on every one sold, before shipping and payment fees. To break even it would need to sell for EUR 8.45 including VAT. It is mostly sold as an add-on, so a price rise is unlikely to cost you many orders.
- **I couldn't work out the Gift Set's margin (SET-GFT-001).** There's no cost for it in cogs.csv. It brought in the most revenue of any product: EUR 642.18 net from 16 sets. After discounts and refunds it averaged EUR 40.14 per set, so it loses money only if a set costs you more than that. I didn't estimate its cost.
- **The other 6 products all make money,** at 44% to 62% gross margin. The Glass Teapot earns the most at EUR 240.76, and the teas have the highest margins at 52% to 62%.

### Worth a look

- Add the Gift Set's unit cost to cogs.csv and I'll rerun the report. That settles the one open question.
- Decide on the Strainer: raise it to at least EUR 8.45, bundle it, or stop selling it.

### Assumptions I made

You didn't get to confirm these first, so correct any that are wrong:
- Unit costs in cogs.csv don't include VAT.
- I left out 3 of the 60 orders:
  - #1013, which is tagged "test".
  - #1021, which was voided.
  - #1042, which was fully refunded.
- I spread the WELCOME10 discounts and the EUR 10 partial refund on #1030 across each order's items by value.
- Shipping, carrier costs and payment fees aren't in the export, so these are margins before those costs.

The export checks out: on every order the items add up to the subtotal, the total equals subtotal minus discount plus shipping, and the tax is 19/119 of the total. Net revenue per product adds up to the order totals.

**Files are in your working folder:**
- `product-profitability-2026-08.xlsx` has these tabs: Summary, Revenue bridge, Excluded orders, Line detail, Raw orders, Raw cogs.
- `product-profitability-2026-08.html` is the report page.
- `build_product_margin.py` rebuilds both. To run a new month, change `PERIOD` at the top.

The report ran and I saved its definition to the skill's `reference/saved_reports.md`. Next month, say "run product profitability" and add the new export.

For the next step, I can run `business-pulse` to show how these margins fit with cash and sales. I can also set this up as a monthly report with `/report-pack`.

<!-- saved for the owner: product-profitability-2026-08.html -->

 
 Product profitability — August 2026 
 PP 
 Which products lose money — August 2026 
 Product profitability · 57 orders · prices ex 19% VAT · Generated [run date] 
 What stands out 
 Steel Strainer sells for EUR 6.50 incl VAT = EUR 5.46 ex VAT, against a unit cost of EUR 7.10. Every one sold loses EUR 1.64 before shipping and fees; 20 units in August 2026 cost you EUR 33.85. Break-even price is EUR 8.45 incl VAT. 
 Gift Set (SET-GFT-001) is missing from cogs.csv, so its margin is n/a. It is the largest product by revenue: EUR 642.18 net from 16 units. It loses money only if it costs more than EUR 40.14 per set (its average net selling price after discounts and refunds). 
 Everything else makes money: 6 products at 44%–62% gross margin. Glass Teapot 600ml earns the most (EUR 240.76). 
 1 Products losing money Steel Strainer: −EUR 33.85 on 20 units 
 EUR 745.71 Gross margin, costed products 45.9% of EUR 1,623.71 net revenue (ex VAT). 
 EUR 642.18 Revenue with no unit cost 28.3% of net merchandise revenue — margin unknown: Gift Set. 
 Margin by product 
 Product Status Units Net revenue 
 COGS Gross margin Margin % Per unit at list 
 Steel Strainer STR-STL-001 Loses money 20 EUR 108.15 EUR 142.00 −EUR 33.85 −31.3% −EUR 1.64 
 Matcha 30g TEA-MAT-030 Profitable 8 EUR 161.34 EUR 77.60 EUR 83.74 51.9% EUR 10.47 
 Green Tea 100g TEA-GRN-100 Profitable 13 EUR 138.76 EUR 53.30 EUR 85.46 61.6% EUR 6.74 
 Ceramic Cup CUP-CER-001 Profitable 14 EUR 210.25 EUR 105.00 EUR 105.25 50.1% EUR 7.63 
 Oolong 50g TEA-OOL-050 Profitable 16 EUR 211.09 EUR 99.20 EUR 111.89 53.0% EUR 7.25 
 Black Tea 100g TEA-BLK-100 Profitable 26 EUR 251.26 EUR 98.80 EUR 152.46 60.7% EUR 5.86 
 Glass Teapot 600ml POT-GLS-600 Profitable 19 EUR 542.86 EUR 302.10 EUR 240.76 44.4% EUR 12.67 
 Gift Set SET-GFT-001 No cost on file 16 EUR 642.18 n/a n/a n/a n/a 
 How this was calculated 
 Net revenue = line price × qty, less its share of discount codes and partial refunds, divided by 1.19 to remove VAT. 
 COGS = units × unit cost from cogs.csv (assumed ex VAT). Partially refunded items keep their cost, since the goods shipped. 
 Left out: #1013 (Tagged 'test'); #1021 (Voided / cancelled (voided)); #1042 (Fully refunded (EUR 60.50)). 
 Shipping charged to customers, carrier costs and payment fees are not in the export, so this is product gross margin before those costs. 
 Not available this run: unit cost for Gift Set (SET-GFT-001), shipping costs, payment processing fees. Generated by Report Builder — Small Business 


<!-- saved for the owner: report_template.html -->

 
 Product profitability — {{PERIOD}} 
 PP 
 Which products lose money — {{PERIOD}} 
 Product profitability · {{ORDERS}} orders · prices ex 19% VAT · Generated {{STAMP}} 
 What stands out 
{{FINDINGS}}
{{TILES}}
 Margin by product 
 Product Status Units Net revenue 
 COGS Gross margin Margin % Per unit at list 
{{ROWS}}
 How this was calculated 
 Net revenue = line price × qty, less its share of discount codes and partial refunds, divided by 1.19 to remove VAT. 
 COGS = units × unit cost from cogs.csv (assumed ex VAT). Partially refunded items keep their cost, since the goods shipped. 
 Left out: {{EXCLUDED}}. 
 Shipping charged to customers, carrier costs and payment fees are not in the export, so this is product gross margin before those costs. 
 Not available this run: unit cost for Gift Set (SET-GFT-001), shipping costs, payment processing fees. Generated by Report Builder — Small Business 

