---
description: Every tool the AI connector offers, what it does and what it needs.
---

# Tool reference

The name in the app (under **Tools this token can use**) is shown first, with the technical tool
name the AI client sees.

## Read tools

| In the app | Tool | What it does | Needs |
| --- | --- | --- | --- |
| **Shop overview** | `get_shop_overview` | Your plan and features, this month's usage against limits, cart counts (live, today, abandoned, ordered, archived), total cart value and widget summary | – |
| **List carts** | `list_carts` | Lists carts in a Dashboard view (all, carts, live, today, week, abandoned, archived, browsing), with search by Cart ID or customer, 20 per page by default (up to 100) | – |
| **Cart details** | `get_cart_details` | One cart: items, totals, customer and addresses, checkout and order state, notes, contact history, linked draft order and activity feed | Activity feed: Basic+ |
| **Analytics** | `get_analytics` | Sessions, carts, value, orders, conversion and a daily breakdown for the last 1 to 90 days (default 60) | Advanced+ |
| **Draft orders** | `list_draft_orders` | Draft orders created in the app, their linked carts, sync status and this month's limit | – |
| **Draft order details** | `get_draft_order` | One draft order in full, plus your store's draft-order metafield definitions | – |
| **Settings** | `get_settings` | Widget, popup, support form and email settings. SMTP credentials are never returned. | – |
| **Search products & customers** | `search_catalog` | Finds products (variant IDs, prices, availability) or customers (IDs, names, emails), up to 50 results | – |

Carts can be identified by any form of Cart ID: text (`v_yna3sj0b2`) or number (`#1024`).

## Write tools

These change data in your store. Leave them unticked on read-only tokens.

| In the app | Tool | What it does | Needs |
| --- | --- | --- | --- |
| **Create draft order** | `create_draft_order_from_cart` | Creates a Shopify draft order from a cart straight away and returns its admin link | Basic+, within your monthly limit |
| **Log contact** | `log_contact` | Adds **Customer contacted us** or **We contacted customer** to a cart, with optional notes | – |
| **Build & manage draft order** | `manage_draft_order` | The full draft builder: create (blank or from a cart), update products, quantities, properties, notes, tags, attributes and metafields, assign, remove or create a customer, and sync to Shopify | Basic+; attributes and properties Advanced+ |

## Prompts

Ready-made instructions for common jobs. In clients that support MCP prompts, choose them from the
prompt menu.

| Prompt | Does |
| --- | --- |
| `abandoned_cart_recovery` | Finds abandoned carts worth following up and suggests next steps |
| `weekly_cart_report` | Summarises the week's carts, value and outcomes |
| `draft_order_followup` | Reviews draft orders that still need action |
| `customize_draft_order` | Walks you through building a draft order step by step, and asks before making any change |
