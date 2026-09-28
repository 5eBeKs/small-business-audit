<!-- small-business / numbers-summary-c / run 1: skill called by name: report-builder; passed -->

## August 2026 sales report

August was your best month of the summer. Net sales were **GBP 85,116**, up 7.2% on July. Most of the growth came from more orders, not bigger ones.

**Net sales (ex VAT)**: GBP 85,116, up 7.2% on July (GBP 79,434) and up 11.2% on June (GBP 76,555)
**Orders shipped**: 1,555, up 5.9% on July (1,468)
**Average order**: GBP 54.74, up 1.2% on July (GBP 54.11)

**For your accountant (August):**

| Line | GBP |
|---|---:|
| Gross sales, ex VAT | 87,503.75 |
| Less discounts | (997.57) |
| Less refunds | (1,389.70) |
| **Net sales, ex VAT** | **85,116.48** |
| Shipping charged, ex VAT (not in revenue) | 2,429.25 |
| VAT collected, after refunds | 17,504.39 |
| Cash taken, including VAT and shipping, after refunds | 105,019.33 |

### What stands out

- **About GBP 3,849 (ex VAT) from 70 pre-orders isn't in August.** These orders were paid between 10 and 31 August but haven't shipped. Your rules only count a sale once it ships, so they'll show up in the month they go out. This also partly explains why Travel Minis Set fell 25.9% against July: it was the most common item on those pre-orders.
- **Refunds more than halved** to GBP 1,390 (1.6% of gross), down from GBP 2,952 (3.5%) in July. Refunds are counted in the month of the original order, though, so returns on late-August orders could still come in and lower August's net figure a little.
- **Eye Balm, Retinol Serum and the Deluxe Gift Box drove the growth.** Retinol Serum was up 20.2% and the Deluxe Gift Box up 18.8%. Eye Balm was up 32.9%. Clay Mask grew fastest at 44.3%.

### Worth a look

- The VAT figure is worked out from the order export. Your accountant should check it against Shopify's own tax report before filing.
- I also left out 8 test orders (GBP 913) and 7 orders that were cancelled before shipping (GBP 900). Both amounts include VAT and shipping. Counting the test orders would have made August look better than it was.

**How I counted:** I used the rules in your `store_definitions.json`. A sale counts once it ships. Figures exclude VAT at 20% and the shipping customers pay. Test orders are left out. A partial refund only takes off the amount refunded, and refunds sit in the month of the order. I checked that the product rows add up exactly to net sales.

**Files in your folder:**
- `August_2026_Sales_Report.xlsx` is the workbook your accountant can check. The tabs are: summary, by product, daily, discount codes, payment methods, excluded orders, a per-order calculation, and the raw export.
- `August_2026_Sales_Report.html` is the report as a web page.
- `build_report.py` is the script that rebuilds the workbook.

**Saved for next month:** I couldn't save the report setup inside the skill's own folder because it's protected. I saved it to `report-definitions.md` in your folder instead. Keep it with your reports, and next month just drop in the new export and say "same report for September." I won't need to ask you anything again.

If you want the full month-end close for your accountant, where your books are checked against Shopify payouts, `/close-month` does that next.

<!-- saved for the owner: August_2026_Sales_Report.html -->

 August 2026 sales report 
 August 2026 sales report 
 Shopify orders, 1–31 Aug 2026, compared with July and June. All figures in GBP, excluding VAT, unless labelled otherwise. 
 What stands out 
 August was the best month of the three. Net sales were GBP 85,116 , up +7.2% on July and +11.2% on June. Most of the growth came from more orders (1,555 shipped, +5.9%). The average order stayed about the same at GBP 54.74. 
 70 pre-orders worth about GBP 3,849 ex VAT were paid in August but haven't shipped, so they're not in August sales. They'll count in the month they ship. Travel Minis Set, which fell 25.9% against July, was the most common item on them (13 orders). 
 Refunds fell to GBP 1,390 (1.6% of gross), from GBP 2,952 in July. Refunds are counted in the month of the order, so returns on late-August orders may still come in and lower this figure. 
 Net sales (ex VAT) GBP 85,116 +7.2% vs July (GBP 79,434) Orders shipped 1,555 +5.9% vs July (1,468) Average order (net) GBP 54.74 +1.2% vs July (GBP 54.11) Refunds (ex VAT) GBP 1,390 1.6% of gross, July 3.5% 
 Gross to net, three months 
 Line Jun 2026 Jul 2026 Aug 2026 Aug vs Jul 
 Gross sales (ex VAT) GBP 79,457.00 GBP 83,389.50 GBP 87,503.75 +4.9% Discounts (ex VAT) (GBP 929.82) (GBP 1,003.11) (GBP 997.57) -0.6% Refunds (ex VAT) (GBP 1,972.18) (GBP 2,952.26) (GBP 1,389.70) -52.9% Net sales (ex VAT) GBP 76,555.00 GBP 79,434.13 GBP 85,116.48 +7.2% Orders shipped 1,339 1,468 1,555 +5.9% Average order value (net, ex VAT) GBP 57.17 GBP 54.11 GBP 54.74 +1.2% Shipping charged (ex VAT, not in revenue) GBP 2,024.38 GBP 2,373.29 GBP 2,429.25 +2.4% VAT collected (goods + shipping, less refunds) GBP 15,710.28 GBP 16,348.10 GBP 17,504.39 +7.1% Cash taken, inc VAT & shipping, less refunds GBP 94,255.75 GBP 98,082.01 GBP 105,019.33 +7.1% 
 Net sales = gross sales minus discounts minus refunds, ex VAT at 20%. Shipping charged to customers is shown separately and isn't in revenue. The VAT figure is worked out from the order export (partial refunds are taken off pro rata). Your accountant should check it against Shopify's own tax report before filing. 
 By product, August vs July 
 Product Units Aug Net Aug Net Jul Change 
 Deluxe Gift Box 105 GBP 6,853.25 GBP 5,767.00 +18.8% Retinol Serum 30ml 221 GBP 6,379.26 GBP 5,305.84 +20.2% Peptide Serum 30ml 180 GBP 5,556.96 GBP 5,467.39 +1.6% Night Cream 50ml 208 GBP 5,060.55 GBP 5,020.23 +0.8% Day Moisturiser 50ml 216 GBP 4,869.64 GBP 4,183.05 +16.4% Vitamin C Serum 30ml 178 GBP 4,620.62 GBP 4,932.90 -6.3% Eye Balm 15ml 258 GBP 4,543.85 GBP 3,419.18 +32.9% Facial Oil 30ml 206 GBP 4,316.44 GBP 3,812.73 +13.2% Gentle Cleanser 250ml 212 GBP 4,128.04 GBP 4,133.06 -0.1% Rose Candle 233 GBP 3,823.30 GBP 3,755.15 +1.8% Mineral SPF 50 216 GBP 3,681.75 GBP 3,519.96 +4.6% Clay Mask 75ml 224 GBP 3,293.48 GBP 2,282.08 +44.3% Travel Minis Set 161 GBP 3,259.14 GBP 4,400.53 -25.9% Starter Gift Box 87 GBP 3,229.62 GBP 3,341.48 -3.3% Coffee Scrub 150ml 220 GBP 2,967.77 GBP 2,931.26 +1.2% Rose Toner 150ml 230 GBP 2,953.08 GBP 2,955.26 -0.1% Body Lotion 200ml 184 GBP 2,843.21 GBP 3,335.03 -14.7% Gentle Cleanser 100ml 235 GBP 2,646.34 GBP 2,413.51 +9.6% Wash Bag 220 GBP 2,636.48 GBP 2,305.39 +14.4% Hand Cream 75ml 238 GBP 2,133.78 GBP 1,722.16 +23.9% Lip Balm Trio 207 GBP 2,008.99 GBP 1,593.88 +26.0% Bamboo Face Towel 206 GBP 1,528.12 GBP 1,419.68 +7.6% Oat Soap Bar 229 GBP 1,405.67 GBP 1,073.29 +31.0% Old Label Serum (clearance) 35 GBP 276.29 GBP 217.60 +27.0% Summer Tin (clearance) 21 GBP 100.87 GBP 126.50 -20.3% Sample Sachet 188 GBP 0.00 GBP 0.00 n/a (GBP 0 item) Total 4,918 GBP 85,116.48 GBP 79,434.13 +7.2% 
 Order discounts and refunds are spread across the items on each order in proportion to their price, so product rows add up exactly to net sales. Sample Sachet is a free item (GBP 0). 
 Left out of August sales 
 Reason Orders Order value (inc VAT & shipping) Cancelled / voided (never shipped) 7 GBP 900.40 Pre-order, paid but not shipped 70 GBP 4,778.30 Test order 8 GBP 912.85 
 Source: Shopify orders export (orders_export.csv, 4,470 orders from 1 Jun to 31 Aug 2026), with the counting rules from store_definitions.json. No live connectors were used. Full detail, every order's calculation and the raw export are in August_2026_Sales_Report.xlsx. 
 

<!-- saved for the owner: report-definitions.md -->

# Report definitions

### Monthly Shopify sales report (for accountant)
Created:   [run date]
Last run:  [run date] (period: August 2026)
Cadence:   monthly (run on request; no schedule set)

```
Report name:  Monthly Shopify sales report
Cadence:      monthly
Period:       prior calendar month (order created date, UK time)
Comparison:   prior month, plus the month before for a 3-month view
Grouping:     product (plus daily, discount code, payment method tabs)

Metrics:
  Gross sales     =  sum of Subtotal (pre-discount) / 1.20                  [Shopify export]
  Discounts       =  sum of Discount Amount / 1.20                          [Shopify export]
  Refunds         =  refunded amount / 1.20; full refunds remove goods only [Shopify export]
  Net sales       =  gross - discounts - refunds (ex VAT, ex shipping)      [Shopify export]
  Orders shipped  =  count of counted orders                                [Shopify export]
  AOV             =  net sales / orders shipped                             [Shopify export]
  Memo lines      =  shipping charged ex VAT, VAT collected (pro rata on refunds), cash taken

Sources:      uploaded file — files/orders_export.csv (+ files/store_definitions.json)
Notes:        Rules from store_definitions.json: test orders excluded (tag 'test' or Bogus Gateway);
              sale counts only when fulfilled (pre-orders / unshipped excluded); ex VAT at 20%;
              customer shipping excluded from revenue; partial refunds deduct amount only;
              refunds attributed to order month. Product rows allocate discounts/refunds pro rata
              to line price and must tie to net sales.
Rerun:        python build_report.py . <Month>_Sales_Report.xlsx YYYY-MM
```

Revisions:

