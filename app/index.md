---
title: "Overview"
description: What CB Customer Cart Manager does, how it works, and the few ideas the rest of the guide relies on.
---

CB Customer Cart Manager gives you live visibility into your shoppers' carts and the tools to help
them finish buying.

## What you get

| Feature | What it does |
| --- | --- |
| **Live cart tracking** | See every visitor session in real time: browsing, cart, checkout, ordered or abandoned, with items, value, customer, location and device. |
| **Cart ID widget** | A small card on your cart page and cart drawer that shows the shopper their Cart ID and a button to send their cart to your support team. |
| **Support tickets** | Shopper requests arrive in the app attached to their cart, with an optional form you design and email alerts to you and the shopper. |
| **Draft orders** | Convert any cart into a Shopify draft order instantly, or customize it first: add products, change quantities, assign a customer, add notes, tags and attributes. |
| **Activity feed** | A timeline of what the shopper did: products viewed, added and removed, checkout started, order completed. |
| **Analytics** | Cart value, cart count, average cart value, draft orders created, top products in carts and customers by location. |
| **AI connector (MCP)** | Let an AI assistant read your carts and create draft orders for you. See [AI connector](/mcp). |

## How it works

1. **A web pixel watches the storefront.** It is installed automatically when you install the
   app. It records page views, product views, add-to-cart and remove-from-cart events, searches and
   checkout starts. You do not need to set anything up for it.
2. **Each visitor gets a cart session.** Sessions move through the statuses **Browsing → Cart →
   Checkout → Ordered**. A cart with no activity for more than an hour counts as **Abandoned**.
   See [Cart statuses and metrics](/app/reference/statuses-and-metrics).
3. **The cart widget shows the Cart ID.** Once you enable the app embed, shoppers see "Your Cart
   ID: …" with a support button. When they press it, a support ticket is created against their
   cart.
4. **You act from the app.** Open the cart, see exactly what they have, log that you contacted
   them, and convert it into a draft order you can send from Shopify.

## Key ideas

**Cart ID.** The identifier shared by you and the shopper. By default it is a text ID such as
`v_yna3sj0b2`. You can switch to simple numbers (`#1`, `#2`, `#3`…). See
[Cart ID format](/app/setup/cart-id-format).

**Tracked carts.** Your plan includes a number of tracked carts per calendar month. Once you reach
it, new carts are not tracked until the next month or until you upgrade. Carts already being
tracked keep updating. See [Plan features](/app/reference/plan-features).

**History retention.** Carts are kept for the number of days your plan allows, then removed from
the dashboard.

**Plans.** Free, Basic, Advanced and Enterprise. Cart tracking starts on Basic. See
[Plans and billing](/app/guides/plans-and-billing).

## Where things are in the app

| Menu item | What you do there |
| --- | --- |
| **Home** (the app name) | Setup Guide, today's numbers, plan usage, session breakdown |
| **Dashboard** | All carts in tabs: live, today, this week, abandoned, support tickets, archived |
| **Draft Orders** | Every draft order created from the app, and new ones from scratch or from a cart |
| **Analytics** | Charts over a date range you pick |
| **Settings** | Widget, visibility, popup and support form, advanced selectors, notifications, MCP |
| **Email Notifications** | SMTP, customer and merchant alerts, email templates |

The app is available in English, German, French, Spanish, Portuguese (Brazilian), Dutch, Italian,
Japanese, Chinese (Simplified), Korean and Filipino. Switch with the **Language** dropdown on the
Home page or in **Settings → General settings**. The storefront widget and emails are in English;
you can change their wording in a [custom template](/app/setup/widget-templates) and in the
[email templates](/app/setup/email-notifications).

Next: [Quickstart](/app/quickstart).
