---
description: How the AI connector protects your store, and how to fix connection problems.
---

# Security and troubleshooting

## How your data is protected

- **Tokens are secret and shown once.** The app stores only a scrambled (hashed) copy, so no one,
  including us, can read your token back.
- **Each token is limited to the tools you chose.** A read-only token cannot change anything.
- **Plan limits still apply.** The assistant cannot do anything your plan does not include.
- **Each token works for your store only.**
- **Rate limits** stop runaway use: 30 requests a minute on Free, 100 on Basic, 300 on Advanced
  and 1,000 on Enterprise.
- **SMTP credentials are never sent** to the assistant.

Remember that anything the assistant reads is sent to the AI provider you use, under that
provider's terms.

## Good practice

- One token per client or person, named clearly.
- Start with **Read-only**, and add write tools only when you need them.
- Set an expiry for tokens used for a one-off job.
- Revoke tokens you no longer use. Check **Last used** to find them.

## Troubleshooting

| Problem | Fix |
| --- | --- |
| The client says unauthorized, or the token is rejected | Check the token was copied in full, with `Bearer ` in front. Check its **Status** is **Active** and not **Expired**. |
| Every token stopped working | MCP may have been turned off. Check **Status** under **Settings → MCP Integration**. |
| "MCP Integration is a premium feature" | MCP is not available on your plan. Click **Upgrade plan**. |
| The assistant says a tool isn't allowed | The token doesn't include that tool. Create a new token with it ticked. |
| The assistant says an upgrade is needed | The action needs a higher plan, for example analytics needs Advanced. |
| Too many requests, try again later | You hit the per-minute rate limit. Wait a minute. |
| Claude Desktop doesn't show the tools | Restart Claude Desktop after editing the config. Check the JSON is valid and Node.js is installed. |
| I lost my token | It can't be shown again. Revoke it and create a new one. |
