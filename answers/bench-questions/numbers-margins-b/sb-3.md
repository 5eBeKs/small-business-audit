<!-- small-business / numbers-margins-b / run 3: skill called by name: report-builder; passed -->

## Product profitability — August 2026

**Only one product loses money: the free Sample Votive.** Every product you charge for sells well above its cost.

**Products losing money:** 1 of 7. The Sample Votive lost USD 9.90 — you gave away 9 at USD 0 and each costs USD 1.10.
**Gross profit:** USD 2,379.31, a 65% margin on USD 3,644.81 of product revenue. That revenue excludes sales tax and shipping.
**Lowest-margin paid product:** Match Cloche at 60%, which still leaves USD 7.20 above cost on every unit.

| Product | Price | Unit cost | Units | Gross profit | Margin |
|---|---:|---:|---:|---:|---:|
| Sample Votive | 0.00 | 1.10 | 9 | (9.90) | n/a |
| Match Cloche | 12.00 | 4.80 | 33 | 237.60 | 60% |
| Wick Trimmer | 14.00 | 5.20 | 27 | 237.60 | 63% |
| Travel Tin Trio | 19.50 | 6.10 | 24 | 319.36 | 69% |
| Fig Candle 8oz | 24.00 | 7.90 | 22 | 347.49 | 67% |
| Cedar Candle 8oz | 24.00 | 7.40 | 27 | 446.23 | 69% |
| Reed Diffuser | 32.00 | 11.20 | 39 | 800.93 | 65% |

### What stands out

- **The votive loss is a giveaway cost, not a pricing problem.** One went into each of 9 orders. If that's intended, it's a USD 9.90 marketing cost for the month.
- **Reed Diffuser earns the most gross profit:** USD 800.93, which is 34% of the month's total.
- **One row in cogs.csv is mistyped.** Cedar Candle's SKU is written `mo-cnd-001 `, in lowercase with a trailing space. Matched as written, it finds no cost, so Cedar Candle would have shown a 100% margin. I matched it to MO-CND-001 for this report. Please correct the sheet.

### Worth a look

- **These figures are gross profit only.** The files have no data on payment processing fees, shipping labels or packaging, so none of those are subtracted. Orders of USD 50 or more shipped free. If a label costs more than about USD 5–7, a free-shipping order made mostly of low-priced items could lose money even though every product clears its cost. To check that, send me a shipping-cost or payouts export.
- **Order #2038 was fully refunded after it had shipped.** If the Cedar Candle and Match Cloche in it weren't returned, that's another USD 12.20 of cost that isn't counted above.

**How I counted:** I used 66 of the 73 orders in the export. I left out 3 orders from July 31, 1 voided order, 2 test orders paid through Bogus Gateway, and the fully refunded order. The SUMMER5 discounts and the USD 12 partial refund on #2049 are spread across each order's items in proportion to price. Summed by product, the rows match the total exactly.

The report ran, and I saved the definition to `report-definitions.md` in your folder rather than inside the plugin, because editing the plugin's saved-reports file needed a permission I didn't have. Keep that file with your reports; drop it into the chat next time and I'll rerun this for any month without asking you anything.

Files are in your working folder:
- `august-product-profitability.xlsx` — tabs: Summary, By product, Exclusions & method, Line detail, Raw orders, Raw cogs
- `august-product-profitability.html` — the report page

**Next step:** run `/report-pack` to repeat this every month with the prior month as the comparison. You could also run `business-pulse` to see how this margin fits the wider business.

<!-- saved for the owner: august-product-profitability.html -->

 
 August product profitability 
 PP Which products lose money — August 2026 
 Product profitability from the Shopify order export and cogs.csv · Generated [run date], 2026 
 What stands out 
 Only the Sample Votive loses money: (USD 9.90). 9 went out free at USD 0 against a USD 1.10 cost, one in each order it shipped with. That's the cost of a giveaway, not a pricing mistake. 
 Every paid product clears 60% gross margin. Match Cloche is the thinnest at 60% (USD 7.20 per unit). Reed Diffuser makes the most gross profit, USD 800.93, which is 34% of the month's total. 
 A formatting slip in cogs.csv would have hidden Cedar Candle's cost. Its row reads mo-cnd-001 (lowercase, with a trailing space). A plain match finds no cost for it and shows 100% margin. I matched it to MO-CND-001 by hand. Please fix the sheet. 
 1 of 7 Products losing money Sample Votive, (USD 9.90) on 9 free units. 
 USD 2,379 Gross profit 65% margin on USD 3,644.81 net product revenue (tax and shipping excluded). 
 60% Lowest paid-product margin Match Cloche. That's still USD 7.20 above cost on every unit. 
 By product, worst first 
 Product Price Unit cost Units Net revenue Gross profit Margin Status 
 Sample Votive MO-SMP-001 USD 0.00 USD 1.10 9 USD 0.00 (USD 9.90) n/a Loses money 
 Match Cloche MO-MAT-001 USD 12.00 USD 4.80 33 USD 396.00 USD 237.60 60% Lowest margin 
 Wick Trimmer MO-WCK-001 USD 14.00 USD 5.20 27 USD 378.00 USD 237.60 63% Profitable 
 Travel Tin Trio MO-CND-010 USD 19.50 USD 6.10 24 USD 465.76 USD 319.36 69% Profitable 
 Fig Candle 8oz MO-CND-002 USD 24.00 USD 7.90 22 USD 521.29 USD 347.49 67% Profitable 
 Cedar Candle 8oz MO-CND-001 USD 24.00 USD 7.40 27 USD 646.03 USD 446.23 69% Profitable 
 Reed Diffuser MO-DIF-001 USD 32.00 USD 11.20 39 USD 1,237.73 USD 800.93 65% Profitable 
 Total 181 USD 3,644.81 USD 2,379.31 65% 
 How this was counted 
 66 of the 73 orders in the export are counted. Left out: 3 orders from July 31 (#1998–2000), 1 voided order (#2008), 2 test orders paid through Bogus Gateway (#2011, #2044) and 1 order that was fully refunded (#2038). 
 Revenue is line price × quantity, before sales tax, less SUMMER5 discounts and the USD 12 partial refund on #2049. Both are spread across each order's items in proportion to price. 
 Gross profit does not include payment fees, shipping labels or packaging, because the files have no data for them. You collected USD 222.40 in shipping charges, and orders of USD 50 or more shipped free. 
 #2038 was fulfilled and then fully refunded. If those items didn't come back, that's another USD 12.20 in cost (a Cedar Candle and a Match Cloche) that isn't counted here. 
 Generated by Report Builder — Small Business · Not available this run: payment fees, shipping costs (not in the files) 


<!-- saved for the owner: report-definitions.md -->

# Report definitions

### Product profitability (which products lose money)
Created:   [run date]
Last run:  [run date]
Cadence:   one-off (can be rerun monthly)

```
Report name:  Product profitability
Cadence:      one-off
Period:       calendar month (first run: August 2026, by order Created at)
Comparison:   none (first run); prior month on rerun
Grouping:     product / SKU

Metrics:
  Net revenue   =  line price x qty, ex sales tax, less order discounts and partial
                   refunds (ex tax), allocated pro rata by line value   [Shopify orders export]
  COGS          =  qty x unit_cost, SKU matched ignoring case and spaces   [cogs.csv]
  Gross profit  =  net revenue - COGS; flag any SKU below zero   [both]
  Gross margin  =  gross profit / net revenue   [both]

Sources:      uploaded files — files/orders_export.csv + files/cogs.csv
Notes:        Owner: prices exclude sales tax. Excluded: orders outside the month,
              voided/cancelled, Bogus Gateway test orders, fully refunded orders.
              Shipping and tax are not product revenue. Payment fees, shipping labels
              and packaging are not in the data, so they are excluded.
              Every SKU on the cost sheet is listed, even with zero sales.
```

