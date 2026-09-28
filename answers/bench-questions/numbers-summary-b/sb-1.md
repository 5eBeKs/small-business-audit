<!-- small-business / numbers-summary-b / run 1: skill called by name: report-builder; passed -->

## Shopify Sales, August 2026

August brought in **USD 4,147.57 across 67 real orders after refunds**. Reed Diffusers made up a third of sales.

**Net merchandise sales:** USD 3,692.00 (gross USD 3,702.00 less USD 10.00 in SUMMER5 discounts)
**Total billed to customers:** USD 4,205.63, less USD 58.06 in refunds, leaves USD 4,147.57
**Average order:** USD 62.77

I can't compare against July: the export only has 3 July orders, all from Jul 31.

### What stands out

- **Reed Diffuser brought in USD 1,248, 34% of merchandise sales** (39 units). That's nearly double the next product, Cedar Candle 8oz (USD 672).
- **34 of 67 orders (51%) shipped free.** Orders of USD 50 or more get free shipping, so you only charged USD 229.35 for shipping. The export doesn't show what you actually paid for postage.
- **Aug 8–14 was the best week, with 20 orders.** Every other full week landed at 13–14.

### For your bookkeeper

| Line | USD |
|---|---:|
| Gross merchandise sales | 3,702.00 |
| Discounts | (10.00) |
| Shipping charged | 229.35 |
| Sales tax collected (owed to the state, not revenue) | 284.28 |
| **Total billed** | **4,205.63** |
| Refunds | (58.06) |
| **Billed less refunds** | **4,147.57** |
| Shopify Payments fees | n/a |

**Left out of the totals:**
- **July orders:** #1998–#2000 were placed Jul 31, so they belong to July.
- **Voided order:** #2008 was voided.
- **Test orders:** #2011 and #2044 (USD 79.25 together) went through the "Bogus Gateway". That's Shopify's test payment method, so no real money came in. If those were real sales, tell me and I'll add them back.

**Worth mentioning to them:**
- **Fees are missing.** The orders export doesn't include Shopify Payments fees or payouts. To match against your bank deposits, they'll need the Shopify Payments payout report.
- **Refunds need a split.** Order #2038 was fully refunded (USD 36.00 of goods, 6.95 shipping and 3.11 tax). Order #2049 got a partial USD 12.00 refund, and the export doesn't say whether that was goods, shipping or tax.
- **One order used a gift card.** #2051 was partly paid with a gift card. The export doesn't say how much, and that portion reduces what you owe on gift cards rather than being new cash.

The totals check out: on every order, the line items add up to the subtotal, and subtotal minus discount plus shipping and tax equals the order total.

### Files (in your working folder)
- **`Shopify_Sales_Report_2026-08.xlsx`** — send this to your bookkeeper. Tabs: Summary, By product, By week, Refunds, Excluded orders, Orders (included), and Raw data (the untouched export).
- **`Shopify_Sales_Report_2026-08.html`** — a report page for reading on screen.
- **`build_august_report.py`** — the script that builds the workbook. It reruns the same way on any month's export.

The report ran, and its definition is saved to **`report-definitions.md`** in your working folder. The plugin's own saved-reports file wasn't writable, so I put it there. Keep that file with your reports; next month, drop in the September export and say "same report", and it will run without any questions.

**Next step:** say "close the month" if you'd like me to match this against your books and Shopify payouts before it goes to the bookkeeper.

<!-- saved for the owner: report-definitions.md -->

# Report definitions

Saved by report-builder. Drop this file back in the chat next time and the report reruns without any questions.

### Monthly Shopify sales
Created:   [run date]
Last run:  [run date] (August 2026)
Cadence:   monthly, on request (no schedule set)

Report name:  Monthly Shopify sales
Cadence:      monthly
Period:       prior calendar month, by order Created at date (store time, -0400)
Comparison:   prior month (only when the export holds a full prior month; else n/a)
Grouping:     product (SKU), week

Metrics:
  Orders                 =  count of orders in period, excl. voided/cancelled and Bogus Gateway tests  [Shopify export]
  Gross merchandise      =  sum of line items (Subtotal)             [Shopify export]
  Discounts              =  sum of Discount Amount                   [Shopify export]
  Net merchandise        =  gross - discounts                        [Shopify export]
  Shipping charged       =  sum of Shipping                          [Shopify export]
  Sales tax collected    =  sum of Taxes (liability, not revenue)    [Shopify export]
  Total billed           =  sum of Total                             [Shopify export]
  Refunds                =  sum of Refunded Amount                   [Shopify export]
  Billed less refunds    =  total billed - refunds                   [Shopify export]
  Average order value    =  total billed / orders                    [Shopify export]
  Processing fees        =  n/a unless a Shopify Payments payout report is supplied

Sources:      uploaded file: Shopify orders export (CSV). Build script: build_august_report.py
              (run: python build_august_report.py files/orders_export.csv 2026-09)
Notes:        For the owner's bookkeeper. The export mixes in orders from the last day of the prior
              month; exclude them by Created at. Order-level fields sit only on the first line of each
              order. Flag gift-card-paid orders and refund splits the export doesn't break out.

Revisions:
  (none)


<!-- saved for the owner: Shopify_Sales_Report_2026-08.html -->

 
 Shopify Sales — August 2026 
 SB 
 Shopify Sales — August 2026 
 Monthly sales report, Aug 1–31 · Built from the Shopify orders export · Generated [run date], 2026 
 August brought in USD 4,147.57 across 67 real orders after refunds. Reed Diffusers made up a third of sales. 
 Reed Diffuser: USD 1,248, 34% of merchandise sales (39 units). That's nearly double the next product, Cedar Candle 8oz (USD 672). 
 34 of 67 orders (51%) shipped free. Every order of USD 50 or more gets free shipping, so shipping charged was only USD 229.35. What you actually paid for postage isn't in this export. 
 Aug 8–14 was the best week, with 20 orders and USD 1,027 billed. Every other full week landed at 13–14 orders. 
 USD 3,692.00 Net merchandise sales Gross USD 3,702.00 less USD 10.00 SUMMER5 discounts. No July comparison available. 
 USD 4,147.57 Billed, less refunds USD 4,205.63 billed less USD 58.06 refunded. Before processing fees. 
 USD 284.28 Sales tax collected Owed to the state, not revenue. 7.25% on goods + shipping. 
 USD 62.77 Average order 67 orders. Free-shipping threshold is USD 50. 
 For the bookkeeper 
 Line August 2026 
 Gross merchandise sales 3,702.00 
 Discounts (10.00) 
 Net merchandise sales 3,692.00 
 Shipping charged 229.35 
 Sales tax collected 284.28 
 Total billed to customers 4,205.63 
 Refunds (#2038 full, #2049 partial) (58.06) 
 Total billed, less refunds 4,147.57 
 Shopify Payments fees n/a 
 Sales by product 
 Product Units Sales (USD) Share 
 Reed Diffuser 39 1,248.00 33.7% 
 Cedar Candle 8oz 28 672.00 18.2% 
 Fig Candle 8oz 22 528.00 14.3% 
 Travel Tin Trio 24 468.00 12.6% 
 Match Cloche 34 408.00 11.0% 
 Wick Trimmer 27 378.00 10.2% 
 Sample Votive (free add-on) 9 0.00 0.0% 
 Total 183 3,702.00 100% 
 By week 
 Week Orders Merchandise (USD) Billed (USD) 
 Aug 1–7 13 717.50 816.33 
 Aug 8–14 20 879.50 1,027.34 
 Aug 15–21 14 852.50 959.03 
 Aug 22–28 14 853.50 960.10 
 Aug 29–31 (3 days) 6 399.00 442.83 
 Total 67 3,702.00 4,205.63 
 Left out of the totals review 
 Order Why Total (USD) 
 #1998, #1999, #2000 Placed Jul 31, so they belong to July 99.57 
 #2008 Voided and cancelled Aug 28 50.35 
 #2011, #2044 Test orders (Bogus Gateway), not real money 79.25 
 Not available this run: Shopify Payments fees and payouts (not in the orders export), July comparison (the export has only 3 July orders), refund split for #2049, gift-card portion of #2051. Every figure ties: line items = subtotals, and subtotal − discount + shipping + tax = total on every order. 

