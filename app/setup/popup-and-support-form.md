---
title: "Popup and support form"
description: Design the form shoppers fill in when they send their cart to support, and optionally show the widget as a popup.
---

**Settings → Popup & Support.** Both features need a paid plan. On Free they are switched off
when you save.

## Support form

When a shopper presses the widget button, you can ask them to fill in a short form first.

**Require customers to fill out a form on submit** is on by default, with one field:

| Label | Type | Required |
| --- | --- | --- |
| Query | Long Text (Message) | Yes |

### Edit the form

- **+ Add Field** adds a new Short Text field.
- For each field set the **Label**, the **Type** and whether it is **Required**.
- **✕ Remove** deletes a field (a form always keeps at least one).

Field types:

| Type | Use for |
| --- | --- |
| Short Text | Name, order number |
| Long Text (Message) | The question itself |
| Email | Where to reply. Used for the [confirmation email](/app/setup/email-notifications). |
| Phone Number | A callback number |
| Dropdown (Select) | A fixed choice. Enter the options separated by commas: `Order, Shipping, Returns` |

> **Add an Email field** if you want to send guests a confirmation email. For signed-in
> customers the app uses their account email; for guests it needs a field of type Email (or one
> labelled "Email").

### What the shopper sees

- **Form on:** a **Contact Support** window with "Reference: Cart ID …", your fields (required ones
  marked \*) and a **Send Request** button. Afterwards: "Your request has been sent successfully!"
- **Form off:** the button sends the cart straight away and changes to **Request Sent!**

Either way, a **Support Request** is added to the cart and appears in the Dashboard's
[Support Tickets](/app/guides/support-tickets) tab.

## Popup

| Setting | Default | What it does |
| --- | --- | --- |
| **Enable Popup Widget** | Off | Shows the widget as a popup, as well as in the cart |
| **Popup Timer Delay (Seconds)** | 1 | How long to wait before the popup opens. Set to 1 to show it immediately after the shopper adds to cart. |
| **Enable Exit-Intent (Show when user tries to leave)** | Off | Opens the popup once when the mouse leaves the top of the window, as a shopper heads for another tab or the close button |

Exit-intent is marked **🔒 Premium** on Free.

Click **Save** in the bar at the top of the page.
