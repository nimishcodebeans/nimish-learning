---
title: "Email variables"
description: The variables you can use in email subjects and content.
---

Use these in the **Subject** or **Content** of an [email template](/app/setup/email-notifications).
In the editor, click a variable under **Liquid variables** to copy it.

<table>
  <thead><tr><th>Variable</th><th>Replaced with</th><th>Example</th></tr></thead>
  <tbody>
    <tr>
      <td><code>&#123;&#123;submission_details&#125;&#125;</code></td>
      <td>Every field the shopper filled in on the support form, with its label</td>
      <td>Query: Can I change the size before I pay?</td>
    </tr>
    <tr>
      <td><code>&#123;&#123;shop_domain&#125;&#125;</code></td>
      <td>Your store's name as in its myshopify address, without <code>.myshopify.com</code></td>
      <td>my-store</td>
    </tr>
    <tr>
      <td><code>&#123;&#123;cart_id&#125;&#125;</code></td>
      <td>The shopper's Cart ID, in your chosen <a href="/app/setup/cart-id-format">format</a></td>
      <td>#1024 or v_yna3sj0b2</td>
    </tr>
  </tbody>
</table>

The editor lists `cart_id` for the **New Support Request** template only, but it works in both.

## Test data

**Preview** and **Send Test Email** fill the variables with sample values: a shopper called John
Doe (`john@example.com`), subject "Need help with order", message "I would like to cancel my last
order.", and Cart ID `#1024`.

## Tip

Put the Cart ID in the merchant alert's subject line, so you can search your inbox for it later:

<pre><code>New request for cart &#123;&#123;cart_id&#125;&#125; on &#123;&#123;shop_domain&#125;&#125;</code></pre>
