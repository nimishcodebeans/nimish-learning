---
title: "Set up and connect"
description: Turn on MCP, create an access token and connect Claude Desktop or any other MCP client.
---

## 1. Turn on MCP

1. Open **Settings → MCP Integration**.
2. If **Status** shows **Disabled**, click **Turn on**.

While MCP is off, every token is rejected.

## 2. Create an access token

1. Under **Create an access token**, give the token a **Token name** that says who or what uses
   it, for example `Claude Desktop — read only`.
2. Under **Tools this token can use**, choose what the assistant may do. All tools are ticked by
   default. Shortcuts:
   - **Select all**
   - **Read-only** ticks only the read tools. Start here if you are unsure.
   - **Clear**
3. Choose an **Expiry**: **Never expires**, **30 days**, **60 days**, **90 days** or **Custom
   date…**.
4. Click **Create token**.

> **Copy your token now.** It is shown only once. Click **Copy token**, or **Copy config** for a
> ready-made Claude Desktop configuration. If you lose it, revoke it and create a new one.

## 3. Connect your client

You need two things from the MCP Integration tab: the **MCP server URL** (click **Copy**) and your
token.

### Claude Desktop

1. In Claude Desktop, open **Settings → Developer → Edit Config**.
2. Paste the configuration from **Copy config**. It looks like this, with your server URL and
   token filled in:

   ```json
   {
     "mcpServers": {
       "cart-manager": {
         "command": "npx",
         "args": ["-y", "mcp-remote", "<MCP server URL>/mcp", "--header", "Authorization:${AUTH}"],
         "env": { "AUTH": "Bearer <YOUR_TOKEN>" }
       }
     }
   }
   ```

   If the file already has an `mcpServers` section, add the `cart-manager` entry inside it.
3. Save the file and restart Claude Desktop.
4. Ask: *"Give me an overview of my store in Cart Manager."*

This setup needs Node.js installed on your computer (for `npx`).

### Other clients (Cursor, ChatGPT, custom agents)

Add a **Streamable HTTP** MCP server:

| Setting | Value |
| --- | --- |
| URL | Your **MCP server URL** |
| Header | `Authorization: Bearer <YOUR_TOKEN>` |

Where to enter this depends on the client; look for "MCP servers" or "connectors" in its
settings.

## 4. Manage your tokens

**Your tokens** lists every token:

| Column | Shows |
| --- | --- |
| **Name** | The name, and the last four characters of the token |
| **Tools** | **All tools** or how many |
| **Expires** | The expiry date, or never |
| **Status** | **Active**, **Disabled** or **Expired** |
| **Last used** | When an assistant last used it, or **Never** |
| **Actions** | **Disable** / **Enable**, **Revoke** |

**Disable** pauses a token and you can enable it again. **Revoke** deletes it for good.
