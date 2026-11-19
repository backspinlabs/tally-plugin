---
name: morning-check
description: The shop's morning check from Tally. Use when someone asks how the shop is doing, for the morning brief, what needs attention today, or how yesterday went across stores.
---

# Morning check

Call `daily_brief` once, with a store's `shop_id` only if one store was asked for (find it with `shop_overview`). Answer from that one result:

1. `for_today` first, in its order and with its names.
2. Yesterday's net sales per store against last week and last year, with each store's `why` where given.
3. The month to date and its pace.
4. What happened yesterday and what stands open, each with its count.

Don't call other tools unless the person asks for the detail behind a line; each line names the tool that has it. If the brief lists anything under `unavailable`, say so in one line.

How to present it: lead with the answer in one or two plain sentences, then one small table per store. Plain language, the few things that matter. End with one line saying when the data was last refreshed.
