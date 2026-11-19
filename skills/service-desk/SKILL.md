---
name: service-desk
description: The service desk's day from Tally. Use for the work order queue, overdue repairs, jobs waiting on parts, how long repairs are taking, or when the shop can take new work in.
---

# Service desk

Three calls, one each:

1. `build_queue` for the next few days, anything overdue first.
2. `waiting_on_parts` for jobs held up, and whether each part is in stock here, at another store, or nowhere.
3. `service_turnaround` for how long jobs have been taking over the last 30 days.

If the question is only how long the wait is, or when a new job can come in, call `service_wait` alone instead.

How to present it: the answer in a sentence or two, then a short list per store. Name the work order number and customer only if this account can see customers. End with when the data was last refreshed.
