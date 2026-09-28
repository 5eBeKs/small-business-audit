<!-- small-business / numbers-margins / run 3: skill called by name: report-builder; passed -->

## Product profitability — August 2026

**One product loses money: the Steel Strainer.** It's the only one with a unit cost on file that sells below cost. I can't say whether the Gift Set loses money, because there's no unit cost for it in cogs.csv. It's also your top product by revenue.

**Steel Strainer gross profit:** EUR −33.85 in August on 20 units, a margin of −31.3%.
**Gross profit on the other six costed products:** EUR 779.56 on EUR 1,515.56 net revenue after VAT, a 51.4% margin. With the Strainer included the total is EUR 745.71 (45.9%).
**Gift Set:** EUR 642.18 net revenue, 28% of all product revenue. Margin is n/a because there's no cost on file.

### What stands out

- **You lose EUR 1.64 on every Steel Strainer sold.** EUR 6.50 including VAT is EUR 5.46 after VAT, and it costs EUR 7.10. Even before VAT, the price is below cost. To break even you'd need to charge at least EUR 8.45 including VAT.
- **The Gift Set needs a cost before anyone can say whether it makes money.** It averaged EUR 40.14 per unit after VAT and discounts, across 16 units. If putting a set together costs you more than that, it's losing money too.
- **The other six products make money, with margins from 44% to 62%.** The Glass Teapot has the thinnest margin (44.4%), but it made the most gross profit of any product: EUR 240.76.

### Worth a look

- **Fix the Strainer price.** Raise it to EUR 8.50 or more, or sell it only in a bundle with a teapot or tea. It's often ordered on its own: #1007 was 3 strainers and nothing else, and #1054 was 2.
- **Send me the Gift Set's unit cost** and I'll fill in its row.

### How I counted it

- **Revenue is after VAT.** I divided prices by 1.19, and the export's Taxes column matches 19% on every order.
- **Discounts and refunds.** WELCOME10 discounts are split across each order's items in proportion to their price. The EUR 10 partial refund on #1030 comes off the Gift Set.
- **Three orders left out:**
  - #1013 was tagged "test".
  - #1021 was voided.
  - #1042 (EUR 60.50) was fully refunded after it shipped. If that stock never came back, it's a loss the report doesn't show.
- **Not included:** payment fees, your shipping costs and packaging aren't in the files, so I didn't subtract them. Including them would push every margin lower and make the Strainer's loss bigger.
- **Totals match.** The per-product rows add up to the EUR 2,265.90 total, and every order's items, discount, shipping and total agree with each other.

I didn't stop to confirm the setup with you first: I assumed a one-off report for August at the product level. Tell me if you want it set up differently.

Files are in the working folder:
- `August-2026-product-profitability.xlsx` has these tabs: Summary, Product margin, Excluded & checks, Order lines (used), Raw orders export, Raw COGS.
- `August-2026-product-profitability.html` is the report page.
- `build_product_margin.py` rebuilds both from a new export.

The report ran, and I saved its definition to the plugin's `saved_reports.md`. Next month, say "run the product profitability report" and drop in September's export.

If you want more:
- **Reorder check:** the restock skill can flag which of these products are also sitting still in stock.
- **How the business is doing overall:** business-pulse gives the picture around these numbers.

<!-- saved for the owner: August-2026-product-profitability.html -->

 
 Product Profitability — August 2026 
 PP 
 Product Profitability — August 2026 
 Which products lose money · Net of 19% VAT · Generated [run date], 2026 
 What stands out 
 The Steel Strainer loses money on every sale. It sells for EUR 6.50 including VAT, which is EUR 5.46 after VAT. It costs EUR 7.10, so you lose EUR 1.64 on each one. In August that added up to EUR 33.85 across 20 units. You'd need to charge at least EUR 8.45 including VAT just to cover the unit cost. 
 No cost is on file for the Gift Set, your top seller. It brought in EUR 642.18 net (28% of product revenue) on 16 units, but SET-GFT-001 isn't in cogs.csv. It averaged EUR 40.14 net per unit, so it only makes money if the set costs less than that to put together. 
 Every other product is healthy, with margins between 44% and 62%. The Glass Teapot has the thinnest margin at 44.4%, but it made the most gross profit of any product: EUR 240.76. 
 EUR (33.85) 
 Steel Strainer gross profit 
 The only product selling below cost: EUR −1.64 per unit on 20 units. 
 EUR 745.71 
 Gross profit, products with a unit cost 
 45.9% of EUR 1,623.71 net revenue. Gift Set not included. 
 EUR 642.18 
 Gift Set net revenue, margin n/a 
 28% of EUR 2,265.90 total net product revenue, with no unit cost on file. 
 By product, worst first 
 Product Units Net rev. ex VAT Unit cost Per unit Gross profit Margin Status 
 Steel Strainer 20 108.15 7.10 (1.64) (33.85) −31.3% Loses money 
 Glass Teapot 600ml 19 542.86 15.90 12.67 240.76 44.4% Profitable 
 Ceramic Cup 14 210.25 7.50 7.63 105.25 50.1% Profitable 
 Matcha 30g 8 161.34 9.70 10.47 83.74 51.9% Profitable 
 Oolong 50g 16 211.09 6.20 7.25 111.89 53.0% Profitable 
 Black Tea 100g 26 251.26 3.80 5.86 152.46 60.7% Profitable 
 Green Tea 100g 13 138.76 4.10 6.74 85.46 61.6% Profitable 
 Gift Set 16 642.18 n/a n/a n/a n/a No cost on file 
 Total 132 2,265.90 745.71 45.9% excl. Gift Set 
 All amounts are in EUR. "Per unit" is the profit at the shelf price, after VAT. Net revenue has discounts and refunds taken off. 
 How this was counted 
 Revenue is net of VAT (price ÷ 1.19). The export's Taxes column matches 19% included in the price on every order. 
 Three orders were left out. #1013 was tagged "test", #1021 was voided, and #1042 (EUR 60.50) was fully refunded. #1042 had already shipped, so if the Black Tea and Gift Set never came back, that stock is also lost. 
 WELCOME10 discounts (EUR 20.28 including VAT, across 6 orders) were split across each order's lines in proportion to their value. The EUR 10.00 partial refund on #1030 was taken off the Gift Set. 
 Shipping charged to customers is left out because it belongs to the order, not a product. Payment fees, your shipping costs and packaging aren't in these files, so they weren't subtracted. Including them would push every margin down and make the Strainer's loss bigger. 
 Not available this run: unit cost for SET-GFT-001, payment fees, fulfilment costs. Source: orders_export.csv and cogs.csv. Generated by Report Builder — Small Business 

