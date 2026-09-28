<!-- small-business / numbers-summary / run 2: skill called by name: report-builder; failed: net-correct, test-order-not-counted -->

## August 2026 Shopify sales

August brought in **EUR 2,461.56 in net revenue excluding VAT**, from 59 orders. Your file only covers August, so I can't compare it with July.

**Gross sales incl. VAT:** EUR 2,999.72 (average order EUR 50.84, 139 units)
**Net sales incl. VAT:** EUR 2,929.22 after EUR 70.50 in refunds, which is 2.4% of gross
**Net VAT at 19%:** EUR 467.66 (EUR 478.92 charged, minus EUR 11.26 on the refunds)

### What stands out

- **Gift Set and Glass Teapot made 52% of item sales:** EUR 833.00 and EUR 646.00 out of EUR 2,868.10. Black Tea sold the most units (27) but brought in only EUR 310.50.
- **Aug 22–28 was your best week at EUR 1,209.60.** That's 40% of the month's sales, from 20 of the 59 orders. The first three weeks averaged about EUR 495 each.
- **Refunds were small.** #1042 was fully refunded (EUR 60.50) and #1030 got EUR 10.00 back. One voided order (#1021, EUR 22.90) is left out of every total.

### For your accountant

| | EUR |
|---|---:|
| Item sales incl. VAT | 2,868.10 |
| + Shipping charged | 151.90 |
| − Discounts (WELCOME10, 6 orders) | (20.28) |
| **Gross sales incl. VAT** | **2,999.72** |
| − Refunds | (70.50) |
| **Net sales incl. VAT** | **2,929.22** |
| − Net VAT 19% | (467.66) |
| **Net revenue excl. VAT** | **2,461.56** |
| Payment processing fees | n/a |

Every order in the export adds up correctly (line items, shipping, discounts and 19% VAT). Payment split: Shopify Payments EUR 2,900.72 (58 orders), PayPal EUR 99.00 (1 order).

### Please check

- **Order #1013 (EUR 80.90) is tagged "test",** but it was paid through Shopify Payments and shipped. I've counted it. If it was a test, gross drops to EUR 2,918.82 and VAT drops by EUR 12.92.
- **Refund dates aren't in the export.** If either refund was made in September, it belongs in September's figures.
- **Your accountant will want the fees too.** They aren't in the orders export. You can get them from the Shopify Payments payout report and your PayPal statement.

### Files

All in your working folder:
- **`August_2026_Shopify_Sales_Report.xlsx`**: a summary tab, then tabs for sales by product, by week, by payment method and adjustments, and your untouched export data on the last tab.
- **`August_2026_Shopify_Sales_Report.html`**: the same report as a page to open in your browser.
- **`build_monthly_sales_report.py`**: the script that builds both files, so next month comes out exactly the same.

I didn't ask you to confirm the setup first because everything could be worked out from your file: calendar August, VAT-inclusive EUR prices, voided orders left out.

The report ran. I couldn't save its setup inside the plugin folder because permission was denied, so it's saved as **`report-definitions.md`** in your working folder instead. Next month, drop in the new export (and that file) and say "same report" — I won't need to ask you anything.

Next step if you want it: **close the month**, which checks these figures against your bookkeeping software and payouts and puts together a closing pack for your accountant.

<!-- saved for the owner: August_2026_Shopify_Sales_Report.html -->

 
 Shopify sales — August 2026 
 Shopify sales — August 2026 
 59 orders · full calendar month · prices include 19% VAT 
 Gift Set and Glass Teapot 600ml made 52% of item sales (EUR 833.00 and EUR 646.00 of EUR 2,868.10). Black Tea 100g moved the most units (27) but brought in EUR 310.50. Aug 22–28 was the peak week at EUR 1,209.60 — 40% of the month from 20 of 59 orders. The first three weeks averaged EUR 495.11. Refunds were EUR 70.50, 2.4% of gross , across 2 orders. Order #1013 (EUR 80.90) is tagged “test” but was paid and fulfilled — counted until you confirm. 
 Gross sales incl. VAT EUR 2,999.72 59 orders · no prior-month baseline in export 
 Net sales incl. VAT EUR 2,929.22 after EUR 70.50 refunds (2.4%) 
 Net VAT (19%) EUR 467.66 EUR 478.92 charged − EUR 11.26 on refunds 
 Net revenue excl. VAT EUR 2,461.56 average order EUR 50.84 · 139 units 
 For the accountant 
 Line EUR 
 Item sales incl. VAT 2,868.10 + Shipping charged 151.90 − Discounts (6 orders) (20.28) 
 Gross sales incl. VAT 2,999.72 
 − Refunds (70.50) 
 Net sales incl. VAT 2,929.22 
 − Net VAT 19% (467.66) 
 Net revenue excl. VAT 2,461.56 
 Payment processing fees n/a 
 Sales by product 
 Product Units Sales incl. VAT Share 
 Gift Set 17 833.00 29.0% Glass Teapot 600ml 19 646.00 22.5% Black Tea 100g 27 310.50 10.8% Ceramic Cup 16 288.00 10.0% Oolong 50g 18 288.00 10.0% Matcha 30g 8 192.00 6.7% Green Tea 100g 14 180.60 6.3% Steel Strainer 20 130.00 4.5% 
 Total 139 2,868.10 100.0% 
 By week 
 Week (paid date) Orders Gross 
 Aug 1–7 10 401.40 Aug 8–14 10 473.60 Aug 15–21 13 610.32 Aug 22–28 20 1,209.60 Aug 29–31 (3 days) 6 304.80 
 Total 59 2,999.72 
 To confirm 
 Item EUR 
 #1013 tagged “test” — counted confirm 80.90 
 #1021 voided — excluded 22.90 
 Refund dates not in export check month 70.50 
 Paid via Shopify Payments (58 orders) 2,900.72 Paid via PayPal Express Checkout (1 orders) 99.00 
 Source: Shopify orders export (files/orders_export.csv), built [run date]. Not available this run: payment processing fees and a prior-month comparison (the export covers August 2026 only). 
 

<!-- saved for the owner: report-definitions.md -->

# Report definitions

### Monthly Shopify sales summary (for the accountant)
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   monthly, on request (owner drops the month's Shopify orders export)

```
Report name:  Monthly Shopify sales summary
Cadence:      monthly, on request
Period:       prior calendar month (by Paid at date)
Comparison:   prior month — n/a until a prior month's export is supplied
Grouping:     product (SKU), week, payment method

Metrics:
  Orders                 =  count of orders, excluding voided          [uploaded Shopify CSV]
  Gross sales incl. VAT  =  sum of order Total = items + shipping − discounts   [CSV]
  Refunds                =  sum of Refunded Amount                     [CSV]
  Net sales incl. VAT    =  gross − refunds                            [CSV]
  Net VAT                =  sum of Taxes − refunds × 19/119            [CSV]
  Net revenue excl. VAT  =  net sales incl. VAT − net VAT              [CSV]
  AOV, units, sales by SKU, sales by week, sales by payment method     [CSV]
  Processing fees        =  n/a — not in the orders export

Sources:      uploaded file — Shopify orders export (orders_export.csv), EUR, prices VAT-inclusive at 19%
Notes:        Voided orders excluded. Orders tagged "test" are counted but flagged for confirmation.
              Refund dates are not in the export; flag them for the accountant.
              Rebuild script: build_monthly_sales_report.py in this folder
              (python build_monthly_sales_report.py <csv> "<Month YYYY>").
```

Revisions:
  (none)

