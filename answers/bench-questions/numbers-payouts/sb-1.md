<!-- small-business / numbers-payouts / run 1: skill called by name: month-end-prep; passed -->

The "missing" money is **EUR 573.88**, and every euro of it is accounted for. Only **EUR 161.39** of it is actually gone: refunds, a chargeback and fees. The rest was never real, went to PayPal instead, or reached your bank in September.

## August: orders to bank

| | EUR |
|---|---:|
| **Order total in the Shopify orders export** (60 orders) | **3,022.62** |
| Test order #1013 (tagged `test`, never charged) | −80.90 |
| Order #1021, cancelled and voided on Aug 16, never charged | −22.90 |
| Order #1055, paid via PayPal, so it isn't in Shopify payouts | −99.00 |
| Refunds: #1042 in full (60.50), #1030 in part (10.00) | −70.50 |
| Chargeback on #1060, sale reversed | −19.30 |
| Card processing fees on 56 charges (about 2%) | −56.59 |
| Chargeback fee on #1060 | −15.00 |
| Aug 30–31 sales (#1050, #1059, #1009, #1058), paid out Sep 1–2 | −209.69 |
| **Paid out to your bank in August** (19 payouts, Aug 3 to Aug 31) | **2,448.74** |

The numbers tie exactly. Every Shopify Payments charge matches its order to the cent, with no duplicates and no charges lacking an order.

## Where it went

- **EUR 103.80 was never real money.** A test order and a voided order are still counted in the orders export. That makes your sales figure too high, not your deposits too low. Leave #1013 out of revenue, or delete it in Shopify.
- **EUR 99.00 went to PayPal.** Check your PayPal balance or PayPal deposits for it.
- **EUR 209.69 is timing.** It was August sales, but the payouts arrived in September. It comes back as a September deposit.
- **EUR 161.39 is actually gone:**
  - EUR 70.50 in refunds
  - EUR 34.30 on the #1060 chargeback (the EUR 19.30 sale plus a EUR 15 fee)
  - EUR 56.59 in normal card fees

  That's about 5% of sales. The chargeback cost almost twice what the order was worth.

## Worth acting on

1. **Chargeback #1060:** Shopify still shows this order as "paid". Check the dispute in Shopify Payments. If it's still open and you have proof of delivery, submit it. Winning usually gets the EUR 19.30 back, and sometimes the fee too.
2. **VAT:** Your prices include VAT. Of the EUR 3,022.62 in orders, EUR 482.58 is VAT (including the test and voided orders). Even the money that landed isn't all yours to spend. Book revenue net of VAT.
3. **Late-July payouts:** The payout export only covers August transactions. Sales from the last few days of July probably paid out in early August, so your bank may show a bit more than EUR 2,448.74. Those deposits belong to July's sales.

## What I couldn't check

I only had the two Shopify exports, not your ledger or bank statement. So I've confirmed orders against payouts, but not payouts against the bank. To check that, tick the 19 August payouts (IDs `PO-20260803` to `PO-20260831`) against your bank statement.

For the full August close, connect your bookkeeping software or send:
- the Profit & Loss report for August
- the transaction detail for August
- the August bank statement

With those I can also run the duplicate scan and receipts check, and build the close packet.
