---
description: Turn a cart into a Shopify draft order instantly, or build a custom one first.
---

# Create draft orders

A draft order is an order you prepare for a customer and send them to pay. Cart Manager builds it
from their cart, so you don't retype anything. Draft orders need **Basic** or above.

There are three ways to create one.

| Way | Where | Use it when |
| --- | --- | --- |
| **Convert to Draft Order** | Cart page | The cart is right as it is |
| **Create Customize Cart** | Cart page | You want to change the cart first |
| **Create New Draft** | Draft Orders page | Starting from scratch, or picking a cart from a list |

## Convert a cart instantly

On the cart page, click **Convert to Draft Order**. A draft order is created in Shopify straight
away, with:

- every item, including line-item properties
- the cart note, or your **Notes & Instructions**
- the cart attributes, plus any you added
- the attached customer, with their email, phone, tags and metafields; or the cart's email if no
  customer is attached

The cart's **Conversion Summary** then shows **Draft Order Generated**, and the draft is listed on
the **Draft Orders** page.

### Keep it in sync

If the shopper keeps changing their cart, click **Update draft order** to copy the latest items
into the draft. The button is active only when the cart and the draft differ. **Go to Draft
Order** opens the draft in Shopify.

## Customize before you create

Click **Create Customize Cart** on the cart page (it says **Edit Customize Cart** if you started
one already). The **Build Draft Order** page opens, pre-filled from the cart.

> Changes here apply only to the draft order. They never change the shopper's live cart.

| Card | What you can do |
| --- | --- |
| **Products** | **Add product** from your catalogue, change quantities, remove lines. **Add Property** edits line-item properties (Advanced and above). |
| **Customer** | Search, attach, create, change or remove the customer. Attaching one brings in their tags and metafields. |
| **Order Details** | **Notes**, and **Cart Attributes** as key and value pairs (Advanced and above) |
| **Tags** | Pick from **Frequently used** or type a new tag and click **Add** |
| **Metafields** | Fill in any draft-order metafields your store has defined |

- **Save** in the top bar keeps your work in the app without creating anything in Shopify yet.
  The draft shows as **Building** on the Draft Orders page, with **Continue Editing**.
- **Create Shopify Draft** (or **Create Draft Order** at the bottom) creates the draft in
  Shopify.
- For a draft that already exists, the button says **Update Shopify Draft** and asks you to
  confirm, because it changes the live draft in Shopify.

## Start from the Draft Orders page

**Draft Orders → Create New Draft**, then choose:

- **Start from Scratch:** a blank draft. Add products and a customer yourself.
- **Pick from Existing Cart:** choose one of your recent active carts that has items, then
  customize it.

## The Draft Orders list

| Column | Shows |
| --- | --- |
| **Cart ID** | The cart it came from, or **New** for a draft started from scratch |
| **Customer** | Email or name, or **Guest** |
| **Draft Order** | The Shopify draft number, or **Building** if not created in Shopify yet |
| **Cart Value** | The draft total |
| **Cart Details** | **View Cart**, **View Draft** (opens it in Shopify), **Customize Draft** |

Search by Cart ID, customer, draft number, product title or SKU, tag or note.

## Send the invoice

Cart Manager creates and updates the draft. Discounts, shipping, payment terms and sending the
invoice happen in Shopify: click **View Draft** or **Go to Draft Order**, then use Shopify's
**Send invoice**.

## Monthly limit

Each plan includes a number of draft orders per month: 10 on Basic, 100 on Advanced, unlimited on
Enterprise. Every draft created from the app counts, whichever way you create it. When you reach
the limit, **Monthly Limit Reached** appears and **Create New Draft** is disabled until next month
or until you upgrade. See [Plan features](../reference/plan-features.md).

If you delete a draft in Shopify, the app unlinks it from the cart, so you can create a new one.
