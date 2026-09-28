<!-- small-business / numbers-summary-b / run 2: skill called by name: report-builder; passed -->

## August 2026 Shopify sales

**August brought in USD 3,692.00 in net product sales from 67 orders. Don't book the raw export total: 6 orders in it aren't August sales.**

- **Net product sales:** USD 3,692.00. That's after USD 10.00 in discounts and excludes shipping and tax. I can't compare it to July because the export only has three July orders.
- **Total collected at checkout:** USD 4,205.63. That includes USD 229.35 in shipping and USD 284.28 in sales tax, which you owe to the state and isn't revenue.
- **Refunds:** USD 58.06 on 2 orders, 1.4% of what was collected. That leaves USD 4,147.57, before processing fees.

### What stands out

- **The raw export overstates August by USD 229.17.** Adding up every order in the file gives USD 4,434.80. It includes 3 orders from July 31 (#1998–#2000), 1 voided order (#2008) and 2 test orders (#2011, #2044, paid through Shopify's test gateway). I left all six out.
- **Reed Diffuser is the top seller** at USD 1,248 (39 units), 34% of product sales and almost double the next product, Cedar Candle at USD 672.
- **The first week was the slowest** at USD 102/day. Every week after that ran USD 122–133/day, about 20% higher. I compared per day because the last week is only 3 days long.

### For your bookkeeper

- **Refund on #2049 (USD 12.00):** the export doesn't show how much of it was tax. Check it in the Shopify admin. The other refund, #2038 (USD 46.06), splits cleanly: USD 36.00 product, USD 6.95 shipping and USD 3.11 tax.
- **Gift card on #2051:** part of this order was paid with a gift card, and the export doesn't show the split. If the gift card was already booked as revenue when you sold it, that part shouldn't be counted again.
- **Not in this export:** Shopify Payments processing fees, what you paid to ship, and product costs. For fees, pull the Shopify Payments payout report.
- **Free shipping:** 34 of 67 orders shipped free, which looks like a USD 50 minimum. Once you have shipping costs, it's worth checking what that costs you.

### Files in your folder

- **`August-2026-Shopify-Sales.xlsx`:** give this one to your bookkeeper. Tabs: Summary, By product, By week, Payment method, Exclusions, and Raw data (the export rows, minus customer emails).
- **`August-2026-Shopify-Sales.html`:** the same report as a page to open in your browser.
- **`report-definitions.md`:** the saved report setup.

I checked the math. Every order's items add up to its subtotal, every order total checks out, and the product and weekly breakdowns match the headline numbers.

I tried to save the report setup in the report tool's own folder but didn't have permission, so it's in `report-definitions.md` in your folder instead. Keep that file and drop it back in next month to rerun this with no questions. If you export September and August together, I can also compare the two months.

**Next step, if useful:** `/close-month` would match these sales against your books and Shopify Payments payouts, which would fill in the missing fees.

<!-- saved for the owner: August-2026-Shopify-Sales.html -->

 
 August 2026 Shopify Sales 
 SR 
 August 2026 Shopify Sales 
 Monthly sales report · Generated [run date] 
 What stands out 
 Summing every order in the export gives USD 4,434.80 , but only USD 4,205.63 is real August sales. The difference is 6 orders: 3 from July 31, 1 voided and 2 test orders. They're listed at the bottom of this page. 
 Reed Diffuser brought in USD 1,248 (34% of product sales), almost double the next product, Cedar Candle at USD 672. 
 Aug 1–7 was the slowest week at USD 102/day . Every week after that ran USD 122–133/day, about 20% higher. 
 The month 
 USD 3,692.00 
 Net product sales 
 After USD 10 in discounts. Excludes shipping and tax. No prior month in the export to compare against. 
 67 
 Orders 
 174 paid units, averaging USD 55.10 per order. 
 USD 58.06 
 Refunds 
 2 orders, 1.4% of the total collected. 
 For the books 
 Line Amount 
 Gross product sales USD 3,702.00 
 Less: discounts (SUMMER5, 2 orders) (USD 10.00) 
 Net product sales USD 3,692.00 
 Shipping charged to customers USD 229.35 
 Sales tax collected Liability USD 284.28 
 Total collected at checkout USD 4,205.63 
 Less: refunds issued (USD 58.06) 
 Total after refunds, before processing fees USD 4,147.57 
 The refund on #2038 (USD 46.06) splits cleanly: USD 36.00 product, USD 6.95 shipping and USD 3.11 tax. The partial refund on #2049 (USD 12.00) doesn't say how much of it was tax, so check that one in the Shopify admin. Shopify Payments fees aren't in the orders export. 
 By product 
 Product Units Gross sales Share 
 Reed Diffuser 39 USD 1,248.00 34% Cedar Candle 8oz 28 USD 672.00 18% Fig Candle 8oz 22 USD 528.00 14% Travel Tin Trio 24 USD 468.00 13% Match Cloche 34 USD 408.00 11% Wick Trimmer 27 USD 378.00 10% Sample Votive 9 USD 0.00 0% 
 Total USD 3,702.00 100% 
 Before the USD 10 of order-level discounts. Sample Votive is a free add-on. 
 By week 
 Week Orders Net product sales Per day 
 Aug 1–7 13 USD 712.50 USD 101.79 Aug 8–14 20 USD 874.50 USD 124.93 Aug 15–21 14 USD 852.50 USD 121.79 Aug 22–28 14 USD 853.50 USD 121.93 Aug 29–31 (3 days) 6 USD 399.00 USD 133.00 
 Aug 29–31 is only 3 days, so compare weeks on the per-day column. 
 Left out of the totals 
 Order Date Reason Total 
 #1998 2026-07-31 Outside period (2026-07-31) USD 33.19 #1999 2026-07-31 Outside period (2026-07-31) USD 33.19 #2000 2026-07-31 Outside period (2026-07-31) USD 33.19 #2008 2026-08-28 Voided / cancelled USD 50.35 #2011 2026-08-11 Test order (Bogus Gateway) USD 20.32 #2044 2026-08-15 Test order (Bogus Gateway) USD 58.93 
 Source: Shopify orders export only. Not available this run: prior-month sales, processing fees, shipping costs, COGS. · Generated by Report Builder — Small Business 


<!-- saved for the owner: report-definitions.md -->

# Report definitions

Saved by Report Builder. Keep this file with your reports; drop it back in the chat and the report reruns without any questions.

---

### Monthly Shopify sales (bookkeeper numbers)
Created:   [run date]
Last run:  [run date] (period: August 2026)
Cadence:   monthly (run on request; no schedule set)

```
Report name:  Monthly Shopify sales
Cadence:      monthly
Period:       prior calendar month, by order Created-at date (store timezone -0400)
Comparison:   prior month (n/a on first run: export held only August + 3 Jul 31 orders)
Grouping:     product (SKU), week of month, payment method

Metrics:
  Gross product sales  =  sum of Subtotal (pre-discount; ties to line qty x price)   [Shopify export]
  Discounts            =  sum of Discount Amount                                    [Shopify export]
  Net product sales    =  gross product sales - discounts                          [Shopify export]
  Shipping charged     =  sum of Shipping                                           [Shopify export]
  Sales tax collected  =  sum of Taxes (liability, not revenue)                     [Shopify export]
  Total collected      =  sum of Total (= net product + shipping + tax)             [Shopify export]
  Refunds              =  sum of Refunded Amount; split product/ship/tax where full [Shopify export]
  Orders, units, AOV   =  count; sum qty on paid lines; net product sales / orders  [Shopify export]

Sources:      uploaded file: Shopify orders export (CSV)
Notes:        Order-level fields sit on the first line of each order only; never sum
              Total across line rows. Exclude orders outside the month, voided or
              cancelled orders, and "Bogus Gateway (for testing)" orders.
              Sample Votive (MO-SMP-001) is a USD 0 add-on; count it separately.
              Processing fees, shipping cost and COGS are not in this export; report n/a.
              Customer emails are dropped from the raw-data tab.
              Tip: export two months at once next time to get a month-over-month comparison.
```

Revisions:
  (none)

