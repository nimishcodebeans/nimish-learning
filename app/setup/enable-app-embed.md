---
title: "Enable the app embed"
description: Switch on the Cb Customer Cart Widget app embed so shoppers see their Cart ID.
---

The cart widget is a Shopify **app embed**. Nothing appears on your storefront until you switch it
on in your theme. It has no settings in the theme editor; everything is configured in the app.

## From the Setup Guide (fastest)

1. Open the app. On **Home**, find the **Setup Guide**.
2. In step **Initial Set Up**, click **Enable App Embed**.
3. The theme editor opens on **App embeds** with **Cb Customer Cart Widget** switched on.
4. Click **Save** in the theme editor.
5. Return to the app. The step shows **Activated** within a few seconds.

## From the theme editor

1. In Shopify admin, go to **Online Store → Themes**, and click **Customize** on your live theme.
2. In the left sidebar, open **App embeds** (the puzzle-piece icon).
3. Switch on **Cb Customer Cart Widget**.
4. Click **Save**.

## Check it works

Open your storefront, add a product to the cart and open the cart page or cart drawer. You should
see a card with **Your Cart ID: …** and a support button.

In the theme editor preview, the widget always shows with a sample ID (`v_preview` or `#1`) and
the popup opens after two seconds, so you can see the design without a real cart.

> **Not showing?** Check, in order:
>
> 1. The embed is on **and saved** in your **live** theme, not a draft theme.
> 2. You are on a page included in [Widget visibility](/app/setup/widget-visibility). The default is the
>    cart page and cart drawer only.
> 3. You are on a paid plan, or its trial, and have not reached your monthly
>    [tracked-cart limit](/app/reference/plan-features). The widget hides for carts that are not
>    tracked.
> 4. If the page is right but the position is wrong, see
>    [Theme compatibility](/app/setup/theme-compatibility).

If you change your theme later, enable the embed again in the new theme.
