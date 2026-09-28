<!-- small-business / numbers-summary-c / run 3: skill called by name: report-builder; failed: revenue-on-the-owners-definitions -->

## August 2026 sales

August was your best month of the three. Net sales were **GBP 85,129**, up 7.1% on July. About a quarter of that increase came from fewer refunds, not from extra sales.

**Net sales (revenue, excluding VAT)**: GBP 85,129.33, up 7.1% on July (GBP 79,460.15) and up 11.2% on June
**Orders shipped**: 1,555, up 5.9% on July (1,468)
**Average order value**: GBP 54.75, up 1.1% on July (GBP 54.13)

### For your accountant (GBP, excluding VAT)

| | June | July | August |
|---|---:|---:|---:|
| Gross product sales | 79,457.00 | 83,389.50 | 87,503.75 |
| Discounts | (929.82) | (1,003.11) | (997.57) |
| Refunds | (1,952.43) | (2,926.25) | (1,376.86) |
| **Net sales** | **76,574.76** | **79,460.15** | **85,129.33** |
| Shipping charged (not in revenue) | 1,971.70 | 2,274.86 | 2,386.78 |
| VAT charged at 20% | 15,709.29 | 16,347.00 | 17,503.22 |
| Customer payments, including VAT | 94,255.75 | 98,082.01 | 105,019.33 |

The figures reconcile: net sales, shipping and VAT add up to customer payments, and the product breakdown adds up to net sales. Shopify's own VAT column comes to GBP 17,504.39 for August. The GBP 1.17 difference is Shopify rounding VAT on each order separately.

### What stands out

- **Refunds halved.** They were GBP 1,377 (1.6% of gross sales), down from GBP 2,926 (3.5%) in July. But refunds are counted in the month the order was placed, so late August returns could still push this up. Re-export before your accountant closes August.
- **Travel Minis Set fell 26%** to GBP 3,259, down GBP 1,141. That's the biggest drop of any product. Eye Balm (+GBP 1,126), Deluxe Gift Box (+GBP 1,086) and Retinol Serum (+GBP 1,073) did most of the growing.
- **GBP 4,778 of August pre-orders isn't included.** These are 70 orders that customers have paid for but you haven't shipped. Your rule is to count a sale when it ships, so they'll count then.

### What I left out and what I assumed

- **Left out of August:** 8 test orders (GBP 913) and 7 cancelled or voided orders (GBP 900), on top of the pre-orders above.
- **Two assumptions your accountant should know about:**
  - The export has no shipping date, so each shipped order counts in the month it was placed.
  - Partial refunds are split between goods and shipping in proportion to the order.

### Files in your folder

- **`sales_report_2026-08.xlsx`**: the workbook. It has a summary tab and a monthly trend, all 26 products, payment methods (for matching against Shopify Payments and PayPal payouts), discount codes, a list of what was left out, and the raw August orders.
- **`sales_report_2026-08.html`**: the same report as a web page. I couldn't publish it as an artifact here, so I saved it as a file you can open in a browser.
- **`build_monthly_sales_report.py`**: the script that builds the workbook. Next month, run it with `2026-09`.

I couldn't save the report definition inside the skill folder because it isn't writable, so it's in **`report-definitions.md`** in this folder. Keep it with your reports. Next month, just ask "how did September go" and I'll run the same report without asking you anything.

Your accountant will probably ask whether your Shopify sales match the ledger. If so, the next step is `/close-month`: it reconciles your Shopify sales against your accounting ledger and prepares the month-end packet for your accountant.

<!-- saved for the owner: report-definitions.md -->

# Report definitions

### Monthly sales summary for the accountant (Shopify)
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   monthly, on request ("how did <month> go", "numbers for my accountant")

Source:     Shopify orders export CSV (files/orders_export.csv). No connector. Shopify is the only revenue source.
Rules:      files/store_definitions.json. VAT-exclusive at 20%. Only shipped orders count, so pre-orders are out.
            Shipping is not revenue. Test orders ('test' tag or Bogus Gateway) are out, and so are cancelled or voided ones.
            Refunds come off by amount only, in the month the order was placed, split between goods and shipping in proportion.
Period:     calendar month, by order Created at date (London time)
Comparison: prior month, with three-month trend
Metrics:    gross product sales, discounts, refunds, net sales (revenue), orders, AOV,
            shipping charged (memo), output VAT (memo), customer receipts incl. VAT
Grouping:   product (discounts and refunds allocated to lines), payment method, discount code, included vs excluded
Build:      python build_monthly_sales_report.py YYYY-MM
            Writes sales_report_YYYY-MM.xlsx. The HTML page is written from its output.

Revisions:
  (none)


<!-- saved for the owner: sales_report_2026-08.html -->

 
 Monthly Sales Summary — August 2026 
 SB 
 Monthly Sales Summary — August 2026 
 Shopify store · Figures ex VAT, GBP · Generated [run date] 2026 
 August net sales were GBP 85,129 , up 7.1% on July and the best of the three months. About a quarter of the increase came from lower refunds. 
 Refunds halved. GBP 1,377 across 45 orders (1.6% of gross sales), down from GBP 2,926 across 83 orders in July (3.5%). August refunds are still coming in, so this figure may rise. They are booked to the month the order was placed. 
 Travel Minis Set is the outlier. GBP 3,259, down 26% (−GBP 1,141). It is the biggest drop in the range. Eye Balm (+GBP 1,126), Deluxe Gift Box (+GBP 1,086) and Retinol Serum (+GBP 1,073) led the growth. 
 GBP 4,778 of August pre-orders is not in these figures. 70 orders were paid but not yet shipped. Under your shipped-only rule, they count when they ship. 
 GBP 85,129 
 Net sales (revenue) 
 +7.1% vs July (GBP 79,460), +11.2% vs June 
 1,555 
 Orders shipped 
 +5.9% vs July (1,468) 
 GBP 54.75 
 Average order value 
 +1.1% vs July (GBP 54.13) 
 GBP 17,503 
 Output VAT 
 On sales and shipping, after refunds. July: GBP 16,347 
 For the accountant: sales, June to August 
 GBP, ex VAT June July August Aug vs Jul 
 Gross product sales 79,457.00 83,389.50 87,503.75 +4.9% 
 Discounts (929.82) (1,003.11) (997.57) −0.6% 
 Refunds (1,952.43) (2,926.25) (1,376.86) −52.9% 
 Net sales (revenue) 76,574.76 79,460.15 85,129.33 +7.1% 
 Shipping charged (kept out of revenue) 1,971.70 2,274.86 2,386.78 +4.9% 
 Output VAT at 20% 15,709.29 16,347.00 17,503.22 +7.1% 
 Customer receipts incl. VAT and shipping 94,255.75 98,082.01 105,019.33 +7.1% 
 Orders counted 1,339 1,468 1,555 +5.9% 
 Net sales + shipping + VAT = customer receipts. Shopify's per-order tax column adds up to GBP 17,504.39 for August. The GBP 1.17 difference is Shopify rounding VAT on each order. 
 Products that moved most, August vs July 
 Product July August Change 
 Eye Balm 15ml 3,419 4,545 +1,126 +33% 
 Deluxe Gift Box 5,767 6,853 +1,086 +19% 
 Retinol Serum 30ml 5,306 6,379 +1,073 +20% 
 Clay Mask 75ml 2,284 3,293 +1,009 +44% 
 Vitamin C Serum 30ml 4,935 4,621 (314) −6% 
 Body Lotion 200ml 3,337 2,843 (493) −15% 
 Travel Minis Set 4,401 3,259 (1,141) −26% 
 GBP ex VAT, after allocating discounts and refunds to each line. All 26 products are in the workbook, and they add up to net sales. 
 What was left out of August 
 Orders placed in August Orders Order value incl. VAT 
 Counted: shipped 1,555 106,722.52 
 Pre-orders paid, not yet shipped 70 4,778.30 
 Test orders (tagged "test" or Bogus Gateway) 8 912.85 
 Cancelled or voided 7 900.40 
 All August orders in the export 1,640 113,314.07 
 The "counted" value is before refunds. Receipts after refunds are GBP 105,019.33. 
 Source: Shopify orders export (orders_export.csv, 1 Jun to 31 Aug 2026), rules from store_definitions.json. No ledger or payment processor connected: n/a. Generated by Report Builder — Small Business 

