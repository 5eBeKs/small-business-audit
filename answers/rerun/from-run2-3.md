<!-- same report as last time, from run 2's saved definition / rerun 3: test order counted -->

## Monthly Shopify sales summary — August 2026

August net revenue was **EUR 2,461.56 excl. VAT** from 59 orders. Nearly two-thirds of the month's sales came in the second half.

**Net revenue excl. VAT:** EUR 2,461.56. There's no comparison with July because I don't have a July export.
**Net sales incl. VAT:** EUR 2,929.22. That's EUR 2,999.72 gross minus EUR 70.50 in refunds, which is 2.4% of gross.
**Net VAT (19%):** EUR 467.66. That's EUR 478.92 charged on orders minus EUR 11.26 of VAT on the refunds.

### What stands out

- **Aug 17–30 brought in EUR 1,937.20 gross, which is 65% of the month.** The two weeks before that (Aug 3–16) brought in EUR 848.42. Both periods are 14 days long, so the second one sold 2.3× as much.
- **Gift Set (EUR 833.00) and Glass Teapot (EUR 646.00) made up 52% of item sales.** Black Tea sold the most units (27) but brought in only EUR 310.50.
- **Order #1013 (EUR 80.90) is tagged "test" but is included in the totals, as your saved rules say.** If it wasn't a real sale, net sales incl. VAT drop to EUR 2,848.32.

### Worth a look

- Confirm whether #1013 was a real sale before this goes to the accountant.
- The export doesn't include refund dates. Check that the refunds on #1030 (EUR 10.00) and #1042 (EUR 60.50) were actually made in August.

Every order passed the integrity checks: line items add up to the subtotal, subtotal + shipping − discounts equals the total, and VAT is 19/119 of the total. Voided order #1021 (EUR 22.90) is excluded.

Not available this run: processing fees (they aren't in the orders export) and the comparison with the prior month (no July export).

**Files** (all in your working folder):
- `Monthly_Sales_Aug_2026.xlsx`: Summary, By product, By week, By payment method, Reconciliation, Flags and Raw data tabs.
- `Monthly_Sales_Aug_2026.html`: the report page, with headline figures, findings and breakdown tables.

**About the saved definition:** it pointed to `build_monthly_sales_report.py`, but that script wasn't in the folder. I rewrote it from your saved spec, so the metrics and rules are the same. It now also builds the weekly, payment-method, reconciliation and flags tabs. I added a revision note to `report-definitions.md`. Keep that file and the script together in this folder, and next month you can just drop in the new export.

If you add July's export too, I'll rerun August with the month-on-month comparison filled in.
