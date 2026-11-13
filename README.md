# The 15-Check Store Ops Daily Checklist

Fifteen checks for Shopify, WooCommerce, Gumroad and Etsy stores. Each one catches a leak that never triggers an alarm — the kind you only discover when a customer complains or a payout is short.

Run this **before** you open analytics. Traffic to a broken store just buys more complaints.

> If more than three boxes are unchecked, stop marketing and fix operations first.

---

## Why a checklist and not a dashboard

Dashboards show you what you already decided to measure. These fifteen checks are the failures that happen *outside* your metrics:

- An order paid but not fulfilled shows up as revenue, not as a problem.
- A chargeback with 48 hours left shows up as nothing at all — until it is lost by default.
- A product page with zero images still counts as "published" in every admin panel.

None of these produce an error, a red badge, or an email. They produce silence, and silence is expensive.

---

## The 15 checks

### Money in transit

**1. Orders paid but not fulfilled in 24h — ship or refund today.**
Paid-and-unfulfilled is the single fastest route to a chargeback. A chargeback costs the sale, the fee, and a strike against your processing account.

**2. Any chargeback or dispute with under 48h left on the response window — answer it before analytics.**
Response windows are counted in calendar days, not business days. Missing one loses the dispute by default, regardless of your evidence.

**3. Payout scheduled but held — read the reason code, not the amount.**
A hold is a signal about your account, not about that one payout. The reason code tells you which document or policy triggered it.

### Deliverability

**4. Email bounce rate above 3% in 7 days — stop sending, authenticate first.**
Sending through a high bounce rate trains filters to distrust your domain. The damage outlasts the campaign.

**5. SPF, DKIM and DMARC passing on a real raw header — not on a tool summary.**
Tool summaries check the record, not the delivery. Open one real message, read the `Authentication-Results` header, and confirm all three pass *aligned* with your From domain.

**6. Any product page with zero images — it is invisible in search, not merely ugly.**
Image-free pages lose both conversion and image-search entry points.

**7. Any product with an empty description — a blank box loses the buyer in about three seconds.**
A price with no explanation is not a product page, it is a question mark.

**8. Checkout tested with a real card in the last 7 days — test mode proves nothing.**
Test mode bypasses the payment processor, the fraud rules, the tax engine and the 3-D Secure step. It proves the button exists, nothing more.

### Policy and support

**9. Refund policy reachable one click from the product page.**
Buried policies read as evasion. One click, visible, in the buyer's language.

**10. Support mailbox answered within 24h — unanswered mail turns into chargebacks.**
A buyer who cannot reach you disputes instead of asking again.

**11. Carrier tracking records older than 30 days still archived.**
Carriers typically purge tracking at 60 days. After that you have no evidence for a late-delivery dispute, even though the dispute can arrive much later.

### Housekeeping

**12. Order export backed up this month.**
Platform outages and account reviews both happen. The export is your only copy that does not depend on someone else's uptime.

**13. Any discount code still live that should have expired.**
Expired-but-live codes leak margin quietly, and affiliate communities find them fast.

**14. Tax or VAT settings changed by a platform without telling you.**
Marketplaces and processors do update tax behaviour. Price checks and invoices will not always flag it.

**15. The one thing you would fix today if you could only fix one.**
Write it down, then fix that one before doing anything else on this list. A checklist you reorder every day is not a system.

---

## How to actually run it

1. Copy this list into a note you open daily, or fork this repo and keep your own answers in a `STATE.md`.
2. Answer each line with **pass**, **fail**, or **unknown**. "Unknown" counts as fail — an unverified control is not a control.
3. Fix fails in order: money in transit → deliverability → policy → housekeeping.
4. Log the date you checked each item. A check without a date is a memory, not evidence.

### Minimal daily version (5 minutes)

If you only have five minutes, do lines 1, 2, 4, 8, and 15. Those five cover most of the money that disappears without a notification.

---

## Automating three of them

Checks 2, 5 and 11 are the ones people ask to automate — chargeback replies, email authentication diagnosis, and tracking-record retention. The automated versions are paid kits from the same author:

- **Chargeback Response Kit** — evidence pack and reply letters by reason code
  <https://475563839418.gumroad.com/l/shopify-chargeback-response-kit>
- **Deliverability Rescue Kit** — SPF/DKIM/DMARC diagnosis and warm-up plan
  <https://475563839418.gumroad.com/l/deliverability-rescue-kit>
- **Launch Readiness Checker** — 60-item pre-launch gate
  <https://475563839418.gumroad.com/l/launch-readiness-checker>

This checklist itself is free, and stays free. There is a downloadable copy (PDF plus a printable one-pager) here:

<https://475563839418.gumroad.com/l/store-ops-daily-checklist>

---

## Contributing

If a check on this list has saved you money, or if there is a leak it misses, open an issue with the store type and what happened. Checks that are specific, verifiable in under five minutes, and silent when skipped get added.

## License

Text released under CC BY 4.0 — copy it, translate it, put it in your own ops doc. Attribution appreciated, not required.
