---
name: stock-to-clear
description: Find slow and aged stock to clear in a Lightspeed shop with Tally. Use when someone asks what isn't selling, what to put on sale, what is tying up money, or what to move between stores.
---

# Stock to clear

1. `slow_movers` with `group_by` brand for the picture by brand, and `slow_movers` on its own for the items tying up the most, largest value first.
2. `stock_age` for how old the stock is, by store and category.
3. `transfer_suggestions` if another store is selling what one store is sitting on.
4. `reorder_point_check` for stock above the maximum the shop set, and for items that still have a reorder point but haven't sold in a year.

If the shop's memory names a category it watches most, look at that category too (`slow_movers` with `category`). If not, ask whether one matters and offer to remember it.

Value at cost when this account can see costs, at retail otherwise, and say which. Name the few brands or items that tie up the most money. These are facts for the shop's decision: don't set prices or markdowns unless asked.
