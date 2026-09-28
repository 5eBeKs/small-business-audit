<!-- small-business / numbers-margins-b / run 2: skill called by name: report-builder; passed -->

## Product profitability — August 2026

**None of the products you charge for lose money.** The only item selling below cost is the free Sample Votive: each one costs you USD 1.10 and brings in nothing.

**Net product revenue:** USD 3,644.00 from 66 orders and 181 units. This excludes tax and shipping, and is after USD 10 of discounts and USD 12 of refunds.
**Gross profit:** USD 2,378.50, a 65.3% margin after USD 1,265.50 of product cost.
**Products below cost:** 1 of 7, the free sample.

There's no earlier month to compare against because this is the first run. July will be the baseline if you rerun it.

### What stands out

- **Sample Votive:** you gave away 9 in August, costing USD 9.90. That's a marketing cost, not a product that's losing money by mistake.
- **Match Cloche** makes the least per unit of anything you charge for: USD 7.20 each (60% margin). It also sells the most units (33).
- **Reed Diffuser** makes the most: USD 800.55, which is 34% of all gross profit, or USD 20.53 a unit.

| Product | Units | Profit / unit | Margin |
|---|---:|---:|---:|
| Sample Votive (free) | 9 | (1.10) | n/a |
| Match Cloche | 33 | 7.20 | 60.0% |
| Wick Trimmer | 27 | 8.80 | 62.9% |
| Travel Tin Trio | 24 | 13.31 | 68.6% |
| Fig Candle 8oz | 22 | 15.78 | 66.6% |
| Cedar Candle 8oz | 27 | 16.52 | 69.1% |
| Reed Diffuser | 39 | 20.53 | 64.7% |

### How I counted

- **Orders left out:** 7 of the 73 in the file.
  - 3 were placed in July (#1998–2000).
  - 1 was voided (#2008).
  - 1 was fully refunded (#2038).
  - 2 were paid through "Bogus Gateway", Shopify's test payment method (#2011, #2044). If those were real sales, tell me and I'll add them back.
- **Discounts and refunds:** the two SUMMER5 discounts and the USD 12 partial refund on #2049 are split across each order's items in proportion to price. The export doesn't say which item was refunded.
- **Revenue:** item price only. Sales tax is excluded, as you said, and so is the USD 222.40 of shipping customers paid.
- **SKU fix:** one entry in `cogs.csv` had a trailing space and was in lowercase (`mo-cnd-001 `). I matched it to Cedar Candle.
- **Totals check:** each order's items add up to its subtotal, and the product rows add up to the total.

### Worth a look

- **Costs not in this data:** payment processing fees, what shipping actually costs you, and packaging. These margins are before those costs. The one place they could turn a sale into a loss is a small order: a single USD 12 Match Cloche with USD 6.95 shipping charged. Send me your shipping and fee costs and I'll work out profit per order, which would show whether those small orders lose money.

**Files:**
- `August-2026-product-profitability.xlsx`: tabs are Summary, By product, Exclusions, Line detail, Raw orders and Raw COGS.
- `August-2026-product-profitability.html`: the report page.

I couldn't save the report definition inside the plugin's folder because I didn't get permission to edit that file. It's in **report-definitions.md** in this folder instead, next to `product_margin.py`, the script that recalculates everything. Keep both with your reports. Next time, drop the definition file back into the chat and I'll rerun the report without asking you anything.

**Next step:** ask me to "run it for September" once that export is ready, and you'll get a month-over-month comparison. You could also run `business-pulse` to see how these margins fit with the rest of the business.

<!-- saved for the owner: August-2026-product-profitability.html -->

 
 Product profitability — August 2026 
 PP 
 Product profitability: August 2026 
 Shopify orders + cost sheet · Generated [run date], 2026 
 No product you charge for loses money. The only item below cost is the free Sample Votive, at USD 1.10 each. 
 Sample Votive: 9 given away, USD 9.90 cost, zero revenue. It works as a promotion, not a product that went wrong. 
 Match Cloche is the thinnest paid item at USD 7.20 profit a unit (60% margin). It also sells the most units (33), often in small orders. 
 Reed Diffuser earns USD 800.55, or 34% of all gross profit, at USD 20.53 a unit. That's the most of any product. 
 USD 3,644 
 Net product revenue 
 66 orders, 181 units. Tax and shipping are excluded. Revenue is after USD 10 of discounts and USD 12 of refunds. 
 USD 2,379 
 Gross profit 
 65.3% margin after USD 1,265.50 of product cost. 
 1 of 7 
 Products below cost 
 Only the free sample. Every paid product keeps at least 60% of its revenue after cost. 
 By product, lowest profit first 
 Product Units Price Unit cost 
 Net revenue Gross profit Margin Per unit 
 Sample Votive 9 0.00 1.10 0.00 (9.90) n/a (1.10) Below cost 
 Match Cloche 33 12.00 4.80 396.00 237.60 60.0% 7.20 Thinnest 
 Wick Trimmer 27 14.00 5.20 378.00 237.60 62.9% 8.80 Profitable 
 Travel Tin Trio 24 19.50 6.10 465.76 319.36 68.6% 13.31 Profitable 
 Fig Candle 8oz 22 24.00 7.90 521.01 347.21 66.6% 15.78 Profitable 
 Cedar Candle 8oz 27 24.00 7.40 645.88 446.08 69.1% 16.52 Profitable 
 Reed Diffuser 39 32.00 11.20 1,237.35 800.55 64.7% 20.53 Profitable 
 Total (USD) 181 3,644.00 2,378.50 65.3% 
 How this was counted 
 The file has 73 orders. 7 were left out : 3 were placed in July (#1998–2000), 1 was voided (#2008), 1 was fully refunded (#2038), and 2 were paid through Shopify's "Bogus Gateway", its test payment method (#2011, #2044). 
 The two SUMMER5 discounts (USD 5 each) and the USD 12 partial refund on #2049 are split across each order's items in proportion to their price. The export doesn't say which item #2049's refund was for. 
 Revenue is item price only. Sales tax is excluded, and so is the USD 222.40 of shipping charged. 
 One cost-sheet SKU had a trailing space and was in lowercase ( mo-cnd-001 ). It was matched to MO-CND-001. 
 Not in this data: payment processing fees, what shipping cost you, packaging. Margins are gross, before these costs. · Generated by Report Builder — Small Business 


<!-- saved for the owner: report-definitions.md -->

# Report definitions

### Product profitability (which products lose money)
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   one-off (rerunnable monthly on request)

```
Report name:  Product profitability
Cadence:      one-off; rerun on request for any month
Period:       calendar month, by order Created at (store-local time)
Comparison:   none (first run); prior month once a second month is run
Grouping:     product (SKU)

Metrics:
  Net revenue   =  qty x line price, less pro-rata share of order discount
                   and partial refund; excl. tax and shipping   [orders_export.csv]
  COGS          =  qty x unit_cost                               [cogs.csv]
  Gross profit  =  net revenue - COGS                            [both]
  Margin        =  gross profit / net revenue                    [both]
  Profit / unit =  gross profit / units                          [both]

Sources:      uploaded files — Shopify orders export + cogs.csv (in files/)
Notes:        Owner: prices exclude sales tax.
              Exclude: orders outside the month, voided/cancelled, fully
              refunded, "Bogus Gateway (for testing)" payments.
              Match SKUs trimmed and case-insensitive (cost sheet has a
              "mo-cnd-001 " entry). Every cost-sheet SKU gets a row, even at zero.
              Processing fees, shipping cost, packaging not in data — margins are gross.
              Script: product_margin.py in this folder
                (python product_margin.py files <output.xlsx>; month is set in the script).
```

Revisions:
  (none)

