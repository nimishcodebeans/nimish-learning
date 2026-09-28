---
title: "Theme compatibility"
description: What to do if the cart widget appears in the wrong place, or not at all, on a custom theme.
---

The widget places itself automatically. It recognises about 150 popular themes, including Dawn
and the other free Shopify themes, Prestige, Impulse, Symmetry, Broadcast, Motion, Warehouse,
Empire, Focal and Kalles. It also finds cart drawers that open without reloading the page.

On a heavily customised or unusual theme, it may not find the right spot. You can tell it where
to go.

## Set custom selectors

**Settings → Advanced → Advanced CSS Selectors.** Leave a field blank to keep auto-detection.

| Field | Where the widget goes | Example |
| --- | --- | --- |
| **Custom Cart Page Selector** | The cart page | `.cart__footer, #cart-form` |
| **Custom Drawer/Sliding Cart Selector** | Inside the cart drawer | `.cart-drawer .drawer__inner` |
| **Custom Popup Selector** | Inside a mini-cart popup | `.mini-cart-popup` |

Each field takes a standard CSS selector for the element the widget should be placed in.

## Find the right selector

1. Open your cart page (or open the drawer) in Chrome.
2. Right-click the area where you want the widget, for example above the checkout button, and
   choose **Inspect**.
3. In the panel that opens, find the surrounding element and note its `class` or `id`.
4. Enter it with a `.` for a class (`.cart__footer`) or `#` for an id (`#cart-form`).
5. Save, then reload your storefront to check.

If you are not comfortable doing this, contact support with your store URL and we will find the
selector for you.
