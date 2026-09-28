<!-- small-business / numbers-margins-c / run 3: skill called by name: report-builder; passed -->

## Product profit: August 2026

Three products lost money in August, **GBP 104 combined**. They are the free sample and your two clearance lines. Every regular product made money, and the thinnest margin was 57%.

**Products at a loss:** 3 of 25. They're the same three that lost money in June and July (the July loss was GBP 107).
**Gross profit, all costed products:** GBP 54,443, up 9% on July (GBP 49,940).
**Not checked:** Peptide Serum, which brought in GBP 5,558 in August. It has no unit cost in `cogs.csv`.

### What stands out

- **Sample Sachet: −GBP 65.80.** You gave away 188 of them at GBP 0.35 each. That's a marketing cost rather than a product that needs fixing, and it's growing: 136 in June, 161 in July, 188 in August.
- **The two clearance lines sell below cost.** Summer Tin is priced at GBP 5.00 before VAT against a GBP 5.80 cost, so it lost GBP 20.93 on 21 units. Old Label Serum is GBP 8.00 against GBP 8.40, so it lost GBP 17.71 on 35 units. Every unit sold loses money even without a discount.
- **Peptide Serum (GL-NEW-001) is missing from `cogs.csv`.** It sold 180 units in August. It would only lose money if each unit cost more than GBP 30.88, so it's almost certainly profitable, but I can't confirm that without the cost.

### Worth a look

- Add Peptide Serum's unit cost to `cogs.csv` and I'll rerun the report.
- If the clearance stock is just being cleared out, the loss is only about GBP 39 a month. If you want those items to at least break even, the price including VAT needs to be at least GBP 6.96 for Summer Tin and GBP 10.08 for Old Label Serum.

### How I worked it out

- **What's included:** shipped orders only, dated by when the order was placed. I left out 70 pre-orders not yet shipped, 7 voided or cancelled orders, and 8 test orders.
- **Revenue:** VAT is removed, shipping is kept out, and discounts and refunds are deducted.
- **Refunds:** I still counted the product cost on refunded orders, because the goods had already shipped. The workbook has a column showing profit if those goods came back and were resold. It doesn't change which products lost money.
- **Not in the data:** payment fees, packaging, shipping costs and ads. These are gross-profit figures, but the margins are high enough that the answer would stay the same.
- **Cleanup:** two SKUs in `cogs.csv` were written slightly differently from the orders export (`gl-ser-030` in lowercase and `GL-MST-050 ` with a trailing space), so I matched them up. The product rows add up exactly to the order-level revenue total.

I also saved the report definition to the skill's `saved_reports.md`, so next month you can just ask "which products lost money in September" without explaining it again.

Next, `business-pulse` can show how these margins sit alongside your cash and sales trend.

Files are in `<run folder>`:
- `product-profit-2026-08.xlsx`
- `product-profit-2026-08.html`

<!-- saved for the owner: product-profit-2026-08.html -->

 Product profit - August 2026 
 Product profit — August 2026 
 Gross profit per product: shipped orders, VAT and shipping stripped out, after discounts and refunds, minus unit cost. Compared with July. 
 What stands out 
 Three products lost money, GBP 104 combined. Sample Sachet GBP (65.80) on 188 given away free; Summer Tin GBP (20.93); Old Label Serum GBP (17.71). All three also lost money in June and July. 
 Both clearance lines are priced below cost. Summer Tin sells for GBP 5.00 ex VAT against a GBP 5.80 cost; Old Label Serum GBP 8.00 against GBP 8.40. Every unit sold loses money before any discount. 
 Peptide Serum can’t be judged — it has no unit cost. GBP 5,558 of August revenue (180 units), and GL-NEW-001 is missing from cogs.csv. It only loses money if it costs more than GBP 30.88 a unit. 
 Products at a loss 3 of 25 Same three as July; Peptide Serum not costed 
 Loss on those three GBP (104.44) July: GBP (106.65) 
 Gross profit, costed products GBP 54,443 up 9% vs July (GBP 49,940) 
 Thinnest regular margin 57% Travel Minis Set; next lowest Wash Bag at 60% 
 Every product, August 
 Product Status Units Net revenue Cost Gross profit Margin vs July 
 Sample Sachet GL-SMP-001 Loss 188 GBP 0 GBP 66 GBP (66) n/a GBP (9) Summer Tin (clearance) GL-CLR-001 Loss 21 GBP 101 GBP 122 GBP (21) -21% GBP 3 Old Label Serum (clearance) GL-CLR-002 Loss 35 GBP 276 GBP 294 GBP (18) -6% GBP 8 Bamboo Face Towel GL-TWL-001 Profit 206 GBP 1,530 GBP 494 GBP 1,035 68% GBP 82 Oat Soap Bar GL-SOP-100 Profit 229 GBP 1,407 GBP 366 GBP 1,041 74% GBP 274 Lip Balm Trio GL-LIP-004 Profit 207 GBP 2,010 GBP 559 GBP 1,451 72% GBP 305 Wash Bag GL-BAG-001 Profit 220 GBP 2,639 GBP 1,056 GBP 1,583 60% GBP 225 Hand Cream 75ml GL-HND-075 Profit 238 GBP 2,134 GBP 547 GBP 1,586 74% GBP 312 Travel Minis Set GL-MIN-001 Profit 161 GBP 3,259 GBP 1,401 GBP 1,858 57% GBP (672) Gentle Cleanser 100ml GL-CLN-100 Profit 235 GBP 2,648 GBP 729 GBP 1,920 72% GBP 183 Starter Gift Box GL-GFT-001 Profit 87 GBP 3,230 GBP 1,174 GBP 2,055 64% GBP 21 Body Lotion 200ml GL-BDY-200 Profit 184 GBP 2,843 GBP 773 GBP 2,070 73% GBP (338) Coffee Scrub 150ml GL-SCR-150 Profit 220 GBP 2,968 GBP 858 GBP 2,110 71% GBP 23 Rose Toner 150ml GL-TNR-150 Profit 230 GBP 2,954 GBP 782 GBP 2,172 74% GBP 11 Clay Mask 75ml GL-MSK-075 Profit 224 GBP 3,293 GBP 851 GBP 2,442 74% GBP 770 Rose Candle GL-CND-001 Profit 233 GBP 3,823 GBP 1,375 GBP 2,449 64% GBP 50 Mineral SPF 50 GL-SPF-050 Profit 216 GBP 3,683 GBP 1,166 GBP 2,516 68% GBP 117 Gentle Cleanser 250ml GL-CLN-250 Profit 212 GBP 4,128 GBP 1,187 GBP 2,941 71% GBP 16 Facial Oil 30ml GL-OIL-030 Profit 206 GBP 4,316 GBP 1,257 GBP 3,060 71% GBP 388 Vitamin C Serum 30ml GL-SER-030 Profit 178 GBP 4,621 GBP 1,406 GBP 3,215 70% GBP (195) Eye Balm 15ml GL-EYE-015 Profit 258 GBP 4,545 GBP 1,316 GBP 3,229 71% GBP 814 Day Moisturiser 50ml GL-MST-050 Profit 216 GBP 4,870 GBP 1,361 GBP 3,510 72% GBP 511 Night Cream 50ml GL-MST-051 Profit 208 GBP 5,061 GBP 1,435 GBP 3,626 72% GBP 82 Deluxe Gift Box GL-GFT-002 Profit 105 GBP 6,853 GBP 2,520 GBP 4,333 63% GBP 798 Retinol Serum 30ml GL-SER-031 Profit 221 GBP 6,379 GBP 2,033 GBP 4,346 68% GBP 724 Peptide Serum 30ml GL-NEW-001 No cost 180 GBP 5,558 n/a n/a n/a 
 Total (costed products) 4918 GBP 85,129 GBP 25,128 GBP 54,443 
 Net revenue total includes Peptide Serum; cost and profit totals exclude it. 
 Not in this data: payment fees, packaging, outbound shipping cost, ad spend — figures are gross profit. Excluded from August: 70 pre-orders not yet shipped (GBP 4,686 incl VAT), 7 voided/cancelled orders and 8 test orders. Product cost is kept on refunded orders. Workbook: product-profit-2026-08.xlsx. Source: files/orders_export.csv + files/cogs.csv (Shopify export, GBP). Built [run date]. 
 
