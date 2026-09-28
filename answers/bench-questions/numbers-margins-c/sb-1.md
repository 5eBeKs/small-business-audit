<!-- small-business / numbers-margins-c / run 1: skill called by name: report-builder; passed -->

## Products that lost money in August 2026

In August, two products sold for less than they cost: the two clearance lines. A third, the free sample sachet, shows a loss because it's given away. These are the same three as in June and July. Together they lost about GBP 104, against GBP 54,431 gross profit on everything else.

| Product | Units | Price ex VAT | Unit cost | Aug profit |
|---|---:|---:|---:|---:|
| Sample Sachet (GL-SMP-001), free giveaway | 188 | GBP 0.00 | GBP 0.35 | (GBP 65.80) |
| Summer Tin, clearance (GL-CLR-001) | 21 | GBP 5.00 | GBP 5.80 | (GBP 20.93) |
| Old Label Serum, clearance (GL-CLR-002) | 35 | GBP 8.00 | GBP 8.40 | (GBP 17.71) |

**Products below cost:** 3 of 26, the same three as June and July.
**Gross profit (products with a cost on file):** GBP 54,431, up 9% on July (GBP 49,914). Revenue after VAT was GBP 85,116.

### What stands out

- **VAT is what hides the clearance losses.** Summer Tin sells for GBP 6.00 and Old Label Serum for GBP 9.60. With VAT included, both look above cost (GBP 5.80 and GBP 8.40). Take the 20% VAT off and they're 80p and 40p a unit under. Moving each price to about GBP 7.00 and GBP 10.10 would break even.
- **Peptide Serum (GL-NEW-001) could be a loss-maker, but I can't tell.** It isn't in cogs.csv. It brought in GBP 5,556.96 on 180 units, so it only loses money if it costs you more than GBP 30.87 a unit. I left its profit as n/a rather than guess.
- **The sample loss is a marketing cost, not a pricing mistake.** It's GBP 65.80 for 188 sachets.

### How it was counted
I used the rules in `store_definitions.json`:
- **Left out:** 8 test orders. Four are tagged "test"; the other four aren't tagged but were paid through Shopify's test gateway, which I also treated as test orders.
- **Only shipped orders count.** That leaves out 70 pre-orders and 7 orders that were voided or refunded before shipping.
- **Revenue:** shipping fees aren't counted. Discount codes and partial refunds are spread across each order's products by value, because the export doesn't say which product a refund was for.
- **Tie-out:** the product rows add up exactly to the order totals, minus shipping and refunds, divided by 1.2.
- **Profit** here doesn't include payment fees, postage, packaging or ads.
- **cogs.csv** has two SKUs typed differently from the export (`gl-ser-030` in lower case, and `GL-MST-050` with a trailing space). I matched them anyway.

### Files (in your working folder)
- `August_2026_product_profit.xlsx` has these tabs: Summary, August by product, June–August trend, excluded orders, rules and assumptions, and both raw files.
- `August_2026_product_profit.html` is the same report as a page to read on screen.

The report ran. The skill folder wasn't writable, so I saved the definition to `report-definitions.md` in this folder. Keep that file with your reports; drop it into the chat next time and I'll rerun this for any month without asking you anything.

**Next step:** send me Peptide Serum's unit cost, or an updated cogs.csv, and I'll confirm whether it's profitable.

<!-- saved for the owner: August_2026_product_profit.html -->

 August 2026 product profit 
 PP Which products lost money in August? Orders created 1–31 Aug 2026 and shipped · revenue ex 20% VAT · generated [run date] 2026 
 What stands out 
 Both clearance lines sell below cost. Summer Tin: GBP 6.00 incl VAT is GBP 5.00 ex VAT, against a GBP 5.80 cost. It lost (GBP 20.93) on 21 units. Old Label Serum: GBP 9.60 is GBP 8.00 ex VAT, against GBP 8.40. It lost (GBP 17.71) on 35 units. Both also lost money in June and July. At the VAT-inclusive price both look profitable, and that is why this is easy to miss. 
 Free sample sachets cost GBP 65.80 (188 given away at GBP 0.35 each). This is a giveaway, not a pricing mistake, but it is the biggest loss line. 
 Peptide Serum can't be judged. It had GBP 5,556.96 revenue on 180 units, but it has no cost in cogs.csv. It only loses money if its unit cost is above GBP 30.87. 
 3 of 26 Products below cost The same three as in June and July. Peptide Serum is unknown. 
 (GBP 104.44) Combined loss July: (GBP 106.65). Small next to GBP 54,431 gross profit. 
 GBP 54,431 Gross profit, costed products Up 9% on July (GBP 49,914). Revenue ex VAT: GBP 85,116. 
 August by product Product Status Units Net price ex VAT Unit cost Revenue ex VAT Profit Margin Sample Sachet GL-SMP-001 Loss (free giveaway) 188 GBP 0.00 GBP 0.35 GBP 0.00 (GBP 65.80) n/a Summer Tin (clearance) GL-CLR-001 Loss 21 GBP 4.80 GBP 5.80 GBP 100.87 (GBP 20.93) -21% Old Label Serum (clearance) GL-CLR-002 Loss 35 GBP 7.89 GBP 8.40 GBP 276.29 (GBP 17.71) -6% Bamboo Face Towel GL-TWL-001 Profit 206 GBP 7.42 GBP 2.40 GBP 1,528.12 GBP 1,033.72 68% Oat Soap Bar GL-SOP-100 Profit 229 GBP 6.14 GBP 1.60 GBP 1,405.67 GBP 1,039.27 74% Lip Balm Trio GL-LIP-004 Profit 207 GBP 9.71 GBP 2.70 GBP 2,008.99 GBP 1,450.09 72% Wash Bag GL-BAG-001 Profit 220 GBP 11.98 GBP 4.80 GBP 2,636.48 GBP 1,580.48 60% Hand Cream 75ml GL-HND-075 Profit 238 GBP 8.97 GBP 2.30 GBP 2,133.78 GBP 1,586.38 74% Travel Minis Set GL-MIN-001 Profit 161 GBP 20.24 GBP 8.70 GBP 3,259.14 GBP 1,858.44 57% Gentle Cleanser 100ml GL-CLN-100 Profit 235 GBP 11.26 GBP 3.10 GBP 2,646.34 GBP 1,917.84 72% Starter Gift Box GL-GFT-001 Profit 87 GBP 37.12 GBP 13.50 GBP 3,229.62 GBP 2,055.12 64% Body Lotion 200ml GL-BDY-200 Profit 184 GBP 15.45 GBP 4.20 GBP 2,843.21 GBP 2,070.41 73% Coffee Scrub 150ml GL-SCR-150 Profit 220 GBP 13.49 GBP 3.90 GBP 2,967.77 GBP 2,109.77 71% Rose Toner 150ml GL-TNR-150 Profit 230 GBP 12.84 GBP 3.40 GBP 2,953.08 GBP 2,171.08 74% Clay Mask 75ml GL-MSK-075 Profit 224 GBP 14.70 GBP 3.80 GBP 3,293.48 GBP 2,442.28 74% Rose Candle GL-CND-001 Profit 233 GBP 16.41 GBP 5.90 GBP 3,823.30 GBP 2,448.60 64% Mineral SPF 50 GL-SPF-050 Profit 216 GBP 17.05 GBP 5.40 GBP 3,681.75 GBP 2,515.35 68% Gentle Cleanser 250ml GL-CLN-250 Profit 212 GBP 19.47 GBP 5.60 GBP 4,128.04 GBP 2,940.84 71% Facial Oil 30ml GL-OIL-030 Profit 206 GBP 20.95 GBP 6.10 GBP 4,316.44 GBP 3,059.84 71% Vitamin C Serum 30ml GL-SER-030 Profit 178 GBP 25.96 GBP 7.90 GBP 4,620.62 GBP 3,214.42 70% Eye Balm 15ml GL-EYE-015 Profit 258 GBP 17.61 GBP 5.10 GBP 4,543.85 GBP 3,228.05 71% Day Moisturiser 50ml GL-MST-050 Profit 216 GBP 22.54 GBP 6.30 GBP 4,869.64 GBP 3,508.84 72% Night Cream 50ml GL-MST-051 Profit 208 GBP 24.33 GBP 6.90 GBP 5,060.55 GBP 3,625.35 72% Deluxe Gift Box GL-GFT-002 Profit 105 GBP 65.27 GBP 24.00 GBP 6,853.25 GBP 4,333.25 63% Retinol Serum 30ml GL-SER-031 Profit 221 GBP 28.87 GBP 9.20 GBP 6,379.26 GBP 4,346.06 68% Peptide Serum 30ml GL-NEW-001 No cost on file 180 GBP 30.87 n/a GBP 5,556.96 n/a n/a 
 Net price is after discount codes and refunds. Rows add up to GBP 85,116.48, which matches order totals minus shipping and refunds, divided by 1.2. 
 How it was counted 
 Left out of August: 8 test orders (4 tagged "test", plus 4 untagged orders paid on the Bogus test gateway), 70 pre-orders not yet shipped, and 7 orders that were voided or refunded before shipping. 
 Shipping fees are not counted as revenue. Discount codes are spread across each order's lines by value. Partial refunds are spread the same way, because the export doesn't say which line was refunded. 
 Profit is revenue ex VAT minus unit cost × units. It leaves out payment fees, postage, packaging and ads. 
 Sources: files/orders_export.csv, files/cogs.csv, files/store_definitions.json · n/a: unit cost for GL-NEW-001 · Generated by Report Builder — Small Business 
 

<!-- saved for the owner: report-definitions.md -->

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

