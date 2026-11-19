---
name: end-of-day
description: Close out a store's day from Tally. Use for end of day, the drawer, payments by type, or whether a day's payments tie to its sales.
---

# End of day

For each store asked for, call `payments_summary` with that store's `shop_id` (from `shop_overview`) and the same date as start and end. Today unless another date was given. With several stores and none named, do each in turn.

Report: sales count, net sales, tax, money collected, each payment type's total (including the shop's own types under `other_payment_types`), refunds paid out, deposits or account payments taken, and whether payments tie to the sales total. If they don't, say so plainly with the difference.

Which of the shop's own payment types count as money (passed as `count_as_money`) comes from the shop's memory. If it doesn't say, ask, and offer to remember the answer.
