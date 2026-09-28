---
title: "Email notifications"
description: Get an email when a shopper sends their cart to support, confirm receipt to the shopper, and optionally send from your own mail server.
---

The app sends two emails, both when a shopper submits the cart widget:

| Email | Sent to | Switch it on in |
| --- | --- | --- |
| **New Support Request** | You | **Merchant Alerts** |
| **Ticket Confirmation** | The shopper | **Customer Alerts** |

Both are **off** after install. Open **Email Notifications** in the app menu (or **Settings →
Notifications → Email Notifications**).

## 1. Alert yourself

**Merchant Alerts** tab.

1. Tick **New support ticket submitted by customer**.
2. In **Notification Email**, enter where alerts should go. It starts with your store email. You
   can enter several addresses separated by commas; the first one receives the email and the rest
   are copied in. Leave it empty to use your store's default email.
3. Click **Save**.

## 2. Confirm to the shopper

**Customer Alerts** tab.

1. Tick **Support ticket submitted (confirmation email)**.
2. Click **Save**.

The shopper needs an email address: either their customer account, or an Email field in your
[support form](/app/setup/popup-and-support-form).

## 3. Edit the templates (optional)

Each tab has a template row: **Ticket Confirmation** under Customer Alerts, **New Support Request**
under Merchant Alerts. Click it to open the editor.

| Part | What you can do |
| --- | --- |
| **Subject** | Plain text. Variables allowed. |
| **Content** | HTML, in a code editor. Variables allowed. |
| **Liquid variables** | Click one to copy it. See [Email variables](/app/reference/email-variables). |
| **Preview** | Shows the email with sample data |
| **Test Email** | Enter a **Recipient Email** and click **Send Test Email**. The template is saved first. |
| **Email Branding** | Tick **Include branding (logo) in this email**, then upload a PNG, JPG, GIF or WebP (max 2MB) or paste an image URL. Each template has its own logo. |
| **Reset to default** | Puts back the original subject and content. This cannot be undone. |

Save with the bar at the top of the page.

Default subjects:

- Ticket Confirmation: `We've received your request! ✉️`
- New Support Request: <code>New Support Request from &#123;&#123;shop_domain&#125;&#125; 🎫</code>

## 4. Use your own mail server (optional)

**SMTP Setup** tab. By default emails go through **CB SMTP Server (Default)**, which needs no
setup.

To send from your own domain, choose **Use Custom SMTP Server** and fill in:

- **Server Details:** host (for example `smtp.sendgrid.net`), port (for example `587`),
  **SMTP Username**, **SMTP Password**, and **Use SSL/TLS (Secure)** if your provider needs it.
- **Sender Identity:** the name and email that appear in the customer's inbox, for example
  "My Store Support" and `support@yourstore.com`.

Sender Identity is used only with a custom SMTP server. Send a test email from a template to check
the connection.
