---
description: Common questions and quick fixes.
---

# FAQ

## Setup

### The widget doesn't appear on my store

Go through these in order:

1. **App embed.** Is **Cb Customer Cart Widget** switched on and saved in your **live** theme?
   See [Enable the app embed](../setup/enable-app-embed.md).
2. **Page.** By default the widget shows on the cart page and in the cart drawer only. Check
   [Widget visibility](../setup/widget-visibility.md), including **Target Audience**.
3. **Plan.** On Free, carts are not tracked, and the widget only shows for tracked carts.
4. **Limit.** If you have reached this month's tracked-cart limit, new carts don't get the widget.
   Check **Home → Plan Usage & Caps**.
5. **Cart Number format.** A new cart gets its number a moment after the first product is
   added. The widget appears once it has one.
6. **Position.** If it appears somewhere odd, or not inside a custom cart drawer, see
   [Theme compatibility](../setup/theme-compatibility.md).

### The Setup Guide step "Initial Set Up" isn't ticked

The app checks your live theme a few seconds after you click **Enable App Embed**. Make sure you
clicked **Save** in the theme editor, then reload the app's Home page.

### I changed my theme

Enable the app embed again in the new theme. Your widget design and settings stay as they are.

### Do I need to install the tracking pixel?

No. It is installed automatically with the app.

## Carts

### A cart I expected isn't in the Dashboard

- Carts appear once they have a Cart ID, a moment after the shopper's first action.
- Visitors who never add to cart show under **All Carts** as **Browsing**, not in the cart tabs.
- Check the **Archived** tab. Someone may have hidden it.
- Carts older than your plan's history retention are removed.
- If you reached your tracked-cart limit, new carts are not tracked.

### Why is a cart "Abandoned" when the shopper is still on my site?

A cart counts as abandoned after an hour with no tracked activity. As soon as the shopper does
something again, it moves back to **Live Carts**.

### How is an order linked to a cart?

Automatically. When the shopper places an order, Shopify tells the app, and the cart is marked
**✓ Order Placed** with a link to the order under **Conversion Summary**.

### Where does the location come from?

It is worked out from the shopper's internet connection, so it is approximate, usually the right
city or a nearby one.

## Draft orders

### Can I add a discount or send an invoice from the app?

Not from the app. Create the draft here, then click **View Draft** to open it in Shopify and add
discounts, shipping or send the invoice. See [Create draft orders](../guides/draft-orders.md).

### "Update draft order" is greyed out

The draft already matches the cart. It becomes active when the cart changes.

### I deleted a draft in Shopify

The app unlinks it from the cart, so you can create a new one.

## Emails

### I'm not getting ticket emails

- Is **New support ticket submitted by customer** ticked, and saved, under **Email Notifications
  → Merchant Alerts**?
- Check **Notification Email** for typos. Separate several addresses with commas.
- Look in spam. Send yourself a test from the template editor.
- With **Custom SMTP**, check your server details with a test email.

### The shopper didn't get a confirmation

Turn on **Support ticket submitted (confirmation email)** under **Customer Alerts**. For guests,
add an **Email** field to your [support form](../setup/popup-and-support-form.md), because the app
needs an address to send to.

## Account

### Can I use the app in another language?

Yes, the app interface is available in 11 languages. Change it with **Language** on Home or in
**Settings → General settings**. For the storefront widget text, create a
[custom template](../setup/widget-templates.md).

### What happens if I uninstall?

The widget disappears from your storefront and Shopify cancels your subscription. If you
reinstall, you choose a plan again.
