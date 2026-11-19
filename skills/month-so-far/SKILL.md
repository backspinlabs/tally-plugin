---
name: month-so-far
description: How the month is going in a Lightspeed shop, from Tally. Use for month-to-date sales, margin, top categories, or how this month compares with last month and last year.
---

# Month so far

Four calls in all:

1. `store_scorecard` with `period` month_to_date and `compare_to` previous_period.
2. The same again with `compare_to` last_year.
3. `profit_by_category` for what made the money.
4. `sales_pace` for where the month is heading.

Don't also call `sales_summary` or `sales_breakdown` for the same numbers.

On margin: lead with the margin on merchandise (`margin_breakdown.merchandise_margin_pct`), give the overall margin as "including labor and service", and if `margin_breakdown` has a note, say how much sold with no cost on file and that it makes the overall margin read high. If this account can't see costs, leave margin out and say so in one line.

How to present it: the answer in one or two sentences, then one small table per store with a total. End with when the data was last refreshed.
