---
description: Exact definitions of cart statuses, dashboard tabs and every number in the app.
---

# Cart statuses and metrics

## Statuses

Every visitor session has one status. It moves forward as the shopper does.

| Status | Badge | Means |
| --- | --- | --- |
| **Browsing** | Browsing | Visiting the store, nothing in the cart yet |
| **Cart** | Cart | Has at least one item in the cart |
| **Checkout** | Checkout | Has started checkout |
| **Ordered** | ✓ Order Placed | Placed an order. The order is linked to the cart automatically. |

## Time-based groups

These are worked out from the cart's **last activity**.

| Group | Rule |
| --- | --- |
| **Live visitor** | Active in the last 5 minutes |
| **Live cart** | Active in the last 30 minutes |
| **Abandoned** | No activity for more than 1 hour, and no checkout completed or order placed |
| **Today** | Active since midnight |
| **Week to date** | Active in the last 7 days |
| **Returning visitor** | Was also active before today. Otherwise **New**. |

## Home page numbers

| Number | Definition |
| --- | --- |
| **Today's Carts** | Carts active today. **Live Carts** below it: active in the last 30 minutes. |
| **Total Cart Value** | Sum of all cart totals in the app, archived carts excluded |
| **Visitors Tracked** | All tracked sessions, carts and browsing |
| **Session Breakdown** | Sessions split into Cart, Abandoned, Ordered, Checkout and Browsing |

## Dashboard numbers

| Number | Definition |
| --- | --- |
| **Today's Visitors** | Sessions active since midnight, split into New and Returning |
| **Today's Carts** | Carts active since midnight |
| **Total cart value** | Sum of all cart totals, archived carts excluded |
| **Total Sales** | Sum of orders placed from tracked carts |

## Plan counters

| Counter | Counts | Resets |
| --- | --- | --- |
| **Tracked carts** | Different real carts with activity this calendar month. Browsing-only visitors do not count. | 1st of the month |
| **Draft orders** | Draft orders created from the app this calendar month | 1st of the month |

## Analytics

| Chart | Definition |
| --- | --- |
| **Total carts value** | Sum of cart totals, by day of last activity |
| **Total carts count** | Carts with at least one item |
| **Average cart value** | Total carts value ÷ Total carts count |
| **Draft Orders created from the app** | Carts linked to a draft order |
| **Top products in carts** | Top five products by quantity in carts |
| **Customers by location** | Top five countries by number of carts |
