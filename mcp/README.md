---
description: Connect Claude, Cursor, ChatGPT or any MCP client to your store's carts and draft orders.
---

# AI connector (MCP)

The AI connector lets an AI assistant work with your Cart Manager data. Instead of scrolling the
Dashboard, you ask:

- *"Which carts were abandoned today, and what was in them?"*
- *"Show me cart #1024 and log that we emailed the customer."*
- *"Turn cart v_yna3sj0b2 into a draft order and add the tag VIP."*
- *"Give me this week's cart report."*

It uses the **Model Context Protocol (MCP)**, an open standard supported by Claude, Cursor, ChatGPT
and many other AI clients.

## What the assistant can do

| Read | Write |
| --- | --- |
| Your plan, usage and cart counts | Create a draft order from a cart |
| List and search carts in every Dashboard view | Log a contact on a cart |
| A cart's full details and activity | Build, edit and sync custom draft orders |
| Analytics (Advanced plan) | |
| Draft orders and their details | |
| Your widget and email settings (never your SMTP password) | |
| Search your products and customers | |

Full list: [Tool reference](tools.md).

The assistant can only do what your plan allows. For example, it cannot create draft orders on
Free or read analytics below Advanced, just as in the app.

## You stay in control

- **Off until you turn it on.** Switch it on in **Settings → MCP Integration**.
- **Tokens per client.** Create a separate access token for each assistant or person.
- **Choose the tools.** Each token can use only the tools you tick, for example read-only.
- **Expiry.** Tokens can expire after 30, 60 or 90 days or on a date you choose.
- **Revoke any time.** Disable or revoke a token, or turn MCP off for the whole store.

More: [Security and troubleshooting](security.md).

## Get started

[Set up and connect](setup.md) takes about five minutes.

Built-in prompts help you start: **abandoned cart recovery**, **weekly cart report**, **draft order
follow-up** and **customize draft order**. In clients that support prompts, pick them from the
prompt menu.
