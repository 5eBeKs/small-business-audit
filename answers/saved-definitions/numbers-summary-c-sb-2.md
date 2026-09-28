# Report definitions

Saved by the report builder. Keep this file with your reports; drop it back in the chat next time and the report reruns without any questions.

### Monthly Shopify sales for the accountant
Created:   [run date]
Last run:  [run date] (period: August 2026)
Cadence:   on request, one calendar month per run (no schedule set)

```
Report name:  Monthly Shopify sales for the accountant
Cadence:      on request
Period:       one calendar month, by order created date (UK time)
Comparison:   prior month (plus the month before, for context)
Grouping:     month; product (SKU); payment method; discount code

Metrics:
  Gross sales       =  sum(Subtotal) / 1.20 (Subtotal is BEFORE discount in this export)   [uploaded CSV]
  Discounts         =  sum(Discount Amount) / 1.20                                          [uploaded CSV]
  Refunds           =  Refunded Amount, applied to goods first (excess = shipping refund), / 1.20   [uploaded CSV]
  Net revenue       =  gross - discounts - refunds (ex VAT, ex shipping)                    [uploaded CSV]
  Shipping income   =  (Shipping - shipping refunds) / 1.20, reported outside revenue       [uploaded CSV]
  Output VAT        =  (net goods + net shipping, incl VAT) / 6                             [uploaded CSV]
  Orders, AOV       =  count of counted orders; net revenue / orders                        [uploaded CSV]

Sources:      uploaded file: Shopify orders export (files/orders_export.csv; one header row per
              order, extra rows per line item) + files/store_definitions.json
Notes:        Rules come from store_definitions.json (owner's answers): count only fulfilled orders;
              exclude test orders (tag 'test' OR 'Bogus Gateway' payment); VAT-exclusive at 20%;
              shipping excluded from revenue; partial refunds by amount; refunds in the order's month.
              Voided orders excluded. Pre-orders (unfulfilled) listed as excluded, not counted.
              Tie-outs: gross - disc - refunds = net; net + shipping + VAT = customer-paid net of refunds.
              No COGS column, so no margin.
```

Revisions:
  (none)
