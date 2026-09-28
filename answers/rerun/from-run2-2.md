<!-- same report as last time, from run 2's saved definition / rerun 2: test order counted -->

## Monthly Shopify sales summary for August 2026

August brought in **EUR 2,461.56 net revenue excluding VAT** from 59 orders. There's no July export in the folder, so these numbers are a starting point for comparison, not a trend.

**Gross sales incl. VAT:** EUR 2,999.72 from 59 orders and 139 units. Prior month is n/a.
**Refunds:** EUR 70.50, which is 2.4% of gross, across 2 orders.
**Net VAT (19%):** EUR 467.66, which is EUR 478.92 of tax collected minus the VAT share of the refunds.
**Average order value:** EUR 50.84.

### What stands out

- **Gift Set is the top product:** EUR 833.00, 29% of product sales. The Glass Teapot is second at EUR 646.00. Together they're half of what you sold.
- **Most sales came in the second half of the month.** The weeks of 17–23 Aug and 24–30 Aug made EUR 1,937 of the EUR 3,000 gross (65%). Each of the first two full weeks made about EUR 400–450.
- **Order #1013 (EUR 80.90) is tagged "test" but was paid and shipped.** I've counted it, as the spec says. Please confirm it was a real sale before your accountant books it.

### Worth a look

- **Refund dates aren't in the Shopify export.** #1042 was fully refunded (EUR 60.50) and #1030 got EUR 10.00 back. Both are counted in August because that's when the orders were paid. Your accountant should check that's the right month.
- **Excluded:** #1021 (EUR 22.90) was voided.
- **Processing fees are n/a** because they aren't in the orders export. If you want them in the report, add the Shopify Payments payout report next time.

All the breakdowns (by product, by week, by payment method) add up to the gross total. The export also matches itself: line items add up to each order's subtotal, and the tax on every order is 19/119 of its total.

**Files are in this folder:**
- **`Monthly_Shopify_Sales_2026-08.xlsx`**: the workbook, with tabs for Summary, Sales by SKU, Sales by week, By payment method, Orders, and Raw data (the full export, unchanged).
- **`Monthly_Shopify_Sales_2026-08.html`**: the report page. Open it in a browser.

Not available this run: a comparison with the previous month (no earlier export) and processing fees (not in the orders export).

---

The report ran and the definition is saved in `report-definitions.md`. The rebuild script it points to, `build_monthly_sales_report.py`, wasn't in the folder anymore. I recreated it from your saved spec, and it's there now for next month.

**Next step:** if you have July's Shopify export, drop it in the files folder and I'll add month-over-month comparisons to this report. Or say "the weekly pack, on schedule" to have `/report-pack` send this out regularly.
