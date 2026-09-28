<!-- small-business / numbers-margins-c / run 2: skill called by name: report-builder; passed -->

## Products that lost money in August 2026

Three products lost money in August, and together they lost GBP 104. Two are clearance lines priced below cost once you take VAT out. The third is free samples.

**Products at a loss:** 3 of 26. July was the same three.
**Total lost on them:** GBP 104.44, against GBP 106.65 in July.
**August gross profit:** GBP 54,443, up 9% on July (GBP 49,940). This leaves out Peptide Serum, which has no unit cost on file.

### What stands out

- **Summer Tin (clearance)** lost GBP 20.93 on 21 units. It sells for GBP 6.00, which is GBP 5.00 without VAT, and it costs GBP 5.80. So every unit loses at least GBP 0.80, and discount codes make it worse. It also lost money in June and July.
- **Old Label Serum (clearance)** lost GBP 17.71 on 35 units. It sells for GBP 9.60, which is GBP 8.00 without VAT, and it costs GBP 8.40. Both clearance lines look profitable if you compare the price customers pay with cost, which is probably how they were priced.
- **Sample Sachets** cost GBP 65.80: 188 were given away free at GBP 0.35 each. That's a marketing cost rather than a pricing mistake, but it's growing (GBP 47.60 in June, GBP 56.35 in July).

### Worth a look

- **Peptide Serum (GL-NEW-001) isn't in cogs.csv**, so I can't tell you whether it made money. It's one of your bigger sellers: GBP 5,558 of August revenue without VAT. It would only lose money if a unit costs more than GBP 30.88, which seems unlikely. Add its cost and I'll rerun.
- Clearance fix: charge at least GBP 6.96 for the Summer Tin and GBP 10.08 for the Old Label Serum to break even. Or accept the loss (about GBP 40 a month) to clear the stock.

### How I counted
- I used your `store_definitions.json` for the rules, so I didn't need to ask you anything.
- **Revenue:** VAT is removed, shipping is left out, and order-level discounts and refunds are spread across the products in each order. Refunds count in the month of the order.
- **Left out of August:** 8 test orders, 6 voided, 1 cancelled, and 70 pre-orders that were paid but not yet shipped.
- **Refunded orders:** their product cost is still counted, because the export doesn't show whether items went back into stock. Leaving that cost out doesn't change which products lost money.
- **Checks:** product revenue adds up to the August total (GBP 85,129). Two SKU codes in cogs.csv had different capitals or a trailing space, and I matched them anyway.

### Files
- **Workbook:** `august-product-profitability.xlsx`. Tabs: Summary, August by product, Profit by month (June to August), Unit economics, Excluded orders, Raw line items.
- **Report page:** `august-product-profitability.html`.

I couldn't save the definition to the skill folder, so it's in `report-definitions.md` in this folder. Keep that file with your reports and drop it back in the chat next time. I'll rerun this for September without asking you anything.

Next step: **"Cash forecast"** runs `cash-flow-snapshot`. Or, for the bigger picture around these numbers, **"How's the business doing?"** runs `business-pulse`.

<!-- saved for the owner: august-product-profitability.html -->

 August product profitability 
 Which products lost money in August 2026 
 Shipped orders, 1-31 Aug 2026. Revenue ex 20% VAT, after discounts and refunds, shipping left out. Compared with July. 
 What stands out 
 Summer Tin (clearance) lost GBP 20.93 on 21 units. It sells for GBP 6.00, which is only GBP 5.00 once you take out VAT. It costs GBP 5.80. Every unit loses at least GBP 0.80. 
 Old Label Serum (clearance) lost GBP 17.71 on 35 units. It sells for GBP 9.60, which is GBP 8.00 ex VAT, against a cost of GBP 8.40. Both clearance lines only look profitable if you compare the VAT-inclusive price with cost. 
 Sample Sachets cost GBP 65.80: 188 given away free at GBP 0.35 each. That's a marketing cost, not a pricing mistake. Peptide Serum has no unit cost in cogs.csv, so its result is unknown. It only loses money if a unit costs more than GBP 30.88. 
 Products at a loss 3 of 26 July: 3 (same three) 
 Total lost on them (GBP 104) July: (GBP 107) 
 August gross profit GBP 54,443 +9% vs July (GBP 49,940), excl. Peptide Serum 
 August by product 
 Product Units Revenue ex VAT COGS Gross profit Margin Profit Jul 
 Peptide Serum 30ml GL-NEW-001 180 GBP 5,558 n/a n/a n/a n/a no cost on file Sample Sachet GL-SMP-001 188 GBP 0 GBP 66 (GBP 66) n/a (GBP 56) loss Summer Tin (clearance) GL-CLR-001 21 GBP 101 GBP 122 (GBP 21) -21% (GBP 24) loss Old Label Serum (clearance) GL-CLR-002 35 GBP 276 GBP 294 (GBP 18) -6% (GBP 26) loss Bamboo Face Towel GL-TWL-001 206 GBP 1,530 GBP 494 GBP 1,035 68% GBP 953 profit Oat Soap Bar GL-SOP-100 229 GBP 1,407 GBP 366 GBP 1,041 74% GBP 767 profit Lip Balm Trio GL-LIP-004 207 GBP 2,010 GBP 559 GBP 1,451 72% GBP 1,146 profit Wash Bag GL-BAG-001 220 GBP 2,639 GBP 1,056 GBP 1,583 60% GBP 1,358 profit Hand Cream 75ml GL-HND-075 238 GBP 2,134 GBP 547 GBP 1,586 74% GBP 1,274 profit Travel Minis Set GL-MIN-001 161 GBP 3,259 GBP 1,401 GBP 1,858 57% GBP 2,530 profit Gentle Cleanser 100ml GL-CLN-100 235 GBP 2,648 GBP 728 GBP 1,920 72% GBP 1,737 profit Starter Gift Box GL-GFT-001 87 GBP 3,230 GBP 1,174 GBP 2,055 64% GBP 2,034 profit Body Lotion 200ml GL-BDY-200 184 GBP 2,843 GBP 773 GBP 2,070 73% GBP 2,408 profit Coffee Scrub 150ml GL-SCR-150 220 GBP 2,968 GBP 858 GBP 2,110 71% GBP 2,087 profit Rose Toner 150ml GL-TNR-150 230 GBP 2,954 GBP 782 GBP 2,172 74% GBP 2,161 profit Clay Mask 75ml GL-MSK-075 224 GBP 3,293 GBP 851 GBP 2,442 74% GBP 1,673 profit Rose Candle GL-CND-001 233 GBP 3,823 GBP 1,375 GBP 2,449 64% GBP 2,399 profit Mineral SPF 50 GL-SPF-050 216 GBP 3,683 GBP 1,166 GBP 2,516 68% GBP 2,399 profit Gentle Cleanser 250ml GL-CLN-250 212 GBP 4,128 GBP 1,187 GBP 2,941 71% GBP 2,925 profit Facial Oil 30ml GL-OIL-030 206 GBP 4,316 GBP 1,257 GBP 3,060 71% GBP 2,672 profit Vitamin C Serum 30ml GL-SER-030 178 GBP 4,621 GBP 1,406 GBP 3,215 70% GBP 3,410 profit Eye Balm 15ml GL-EYE-015 258 GBP 4,545 GBP 1,316 GBP 3,229 71% GBP 2,414 profit Day Moisturiser 50ml GL-MST-050 216 GBP 4,870 GBP 1,361 GBP 3,510 72% GBP 2,999 profit Night Cream 50ml GL-MST-051 208 GBP 5,061 GBP 1,435 GBP 3,626 72% GBP 3,544 profit Deluxe Gift Box GL-GFT-002 105 GBP 6,853 GBP 2,520 GBP 4,333 63% GBP 3,535 profit Retinol Serum 30ml GL-SER-031 221 GBP 6,379 GBP 2,033 GBP 4,346 68% GBP 3,622 profit 
 Left out: 8 test orders, 6 voided, 1 cancelled, 70 paid but not yet shipped (pre-orders). COGS counts all shipped units, including units on refunded orders, because the export doesn't show restocks. Leaving those out doesn't change which products lost money. Not available: unit cost for GL-NEW-001 Peptide Serum. 
 

<!-- saved for the owner: report-definitions.md -->

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

