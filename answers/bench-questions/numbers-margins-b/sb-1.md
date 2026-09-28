<!-- small-business / numbers-margins-b / run 1: skill called by name: report-builder; passed -->

## Which products lose money: August 2026

**Only one product lost money: the free Sample Votive.** Every product you charge for made a profit, with gross margins between 59% and 69%.

**Net product revenue**: USD 3,644.00 across 67 orders. That's before tax, after USD 10.00 in discounts and USD 48.00 in refunds.
**Gross profit**: USD 2,366.30, a 65% margin on USD 1,277.70 of product cost.
**Products below cost**: 1 of 7. The Sample Votive lost USD 9.90.

| Product | Units | Net revenue | Cost of goods | Gross profit | Margin |
|---|--:|--:|--:|--:|--:|
| Sample Votive | 9 | USD 0.00 | USD 9.90 | **USD (9.90)** | n/a |
| Match Cloche | 34 | USD 396.00 | USD 163.20 | USD 232.80 | 59% |
| Wick Trimmer | 27 | USD 378.00 | USD 140.40 | USD 237.60 | 63% |
| Travel Tin Trio | 24 | USD 465.76 | USD 146.40 | USD 319.36 | 69% |
| Fig Candle 8oz | 22 | USD 521.01 | USD 173.80 | USD 347.21 | 67% |
| Cedar Candle 8oz | 28 | USD 645.88 | USD 207.20 | USD 438.68 | 68% |
| Reed Diffuser | 39 | USD 1,237.35 | USD 436.80 | USD 800.55 | 65% |

### What stands out
- **The Sample Votive** goes out at USD 0.00 and costs USD 1.10 each. You gave away 9 in August, so it's a USD 9.90 marketing cost rather than a pricing problem.
- **The Match Cloche has the lowest margin** of anything you sell, at 59% (USD 12.00 price against USD 4.80 cost). A USD 12.00 refund also came off it. It's still comfortably profitable.
- **The Reed Diffuser brings in the most profit**: USD 800.55, about a third of the total.

### What I left out or adjusted
- **I excluded 6 orders:** 3 dated July 31, 2 test orders paid through Shopify's test gateway (#2011, #2044), and 1 voided order (#2008).
- **Refunds:** order #2038 was fully refunded, so its revenue is zero. I still counted its product cost because the items had shipped. The USD 12.00 partial refund on #2049 is spread across that order's items in proportion to their value.
- **The cost sheet** lists `mo-cnd-001 ` in lowercase with a trailing space. I matched it to Cedar Candle anyway, and every product sold has a cost.

### Worth a look
These figures are product margin only. **What you paid carriers for shipping and your card processing fees aren't in the export.** 34 of 67 orders shipped free (the pattern suggests free shipping over USD 50), and small orders carry the highest shipping cost relative to their value. So the real loss-maker is more likely a single USD 12.00 Match Cloche or USD 14.00 Wick Trimmer order that ships for USD 6.95 than any one product. If you can export your August shipping labels and payout fees, I'll add them and show profit per order.

### Files
In your working folder:
- **`product_profitability_2026-08.xlsx`**: a summary tab, a by-product tab, line-by-line detail, a tab listing the excluded orders, and the raw data.
- **`product_profitability_2026-08.html`**: the same report as a formatted page.
- **`build_product_profitability.py`**: reruns the report for any month, e.g. `python build_product_profitability.py 2026-09`.

The definition is saved to the skill's `saved_reports.md`, so asking for "the product profitability report for September" will rerun it without any setup questions.

Next step, if you'd like: bring in shipping and fee costs to get profit per order. Or I can run `inventory-planner` to see which of these products you should reorder.

<!-- saved for the owner: product_profitability_2026-08.html -->

 
 Product profitability — 2026-08 
 MO Which products lose money — August 2026 
 Product profitability · 67 orders · Generated [run date] 
 What stands out 
 Only the free Sample Votive loses money : 9 given away at USD 1.10 each = USD (9.90). Every product you actually charge for is profitable at list price. 
 Match Cloche has the thinnest paid margin at 59% (USD 12.00 price vs USD 4.80 cost) — still well above water. 
 Reed Diffuser earns the most : USD 800.55 gross profit on 39 units, 65% margin. 
 USD 3,644.00 Net product revenue Pre-tax, after USD 10.00 discounts and USD 48.00 refunds 
 USD 2,366.30 Gross profit 65% margin on USD 1,277.70 product cost 
 1 of 7 Products below cost Sample Votive: USD (9.90) 
 By product, worst first 
 Product Units Net revenue COGS Gross profit Margin Status 
 Sample Votive MO-SMP-001 9 USD 0.00 USD 9.90 USD (9.90) — Loses money Match Cloche MO-MAT-001 34 USD 396.00 USD 163.20 USD 232.80 59% Profitable Wick Trimmer MO-WCK-001 27 USD 378.00 USD 140.40 USD 237.60 63% Profitable Travel Tin Trio MO-CND-010 24 USD 465.76 USD 146.40 USD 319.36 69% Profitable Fig Candle 8oz MO-CND-002 22 USD 521.01 USD 173.80 USD 347.21 67% Profitable Cedar Candle 8oz MO-CND-001 28 USD 645.88 USD 207.20 USD 438.68 68% Profitable Reed Diffuser MO-DIF-001 39 USD 1,237.35 USD 436.80 USD 800.55 65% Profitable Total 183 USD 3,644.00 USD 1,277.70 USD 2,366.30 65% 
 What this doesn't include Product-level gross profit only. Shipping charged (USD 229.35) is left out of revenue; what you paid carriers isn't in the export, and 34 of 67 orders shipped free. Payment-processing fees aren't in the export either. Excluded: outside period (2026-07-31) (3), test order (bogus gateway) (2), voided / cancelled (1). 
 Sources: files/orders_export.csv, files/cogs.csv. Not available this run: carrier shipping cost, payment processing fees. 
 
