# Contributing to the Cart Manager docs

This repo is the source of the public documentation for CB Customer Cart Manager. It is plain
Markdown, so it works with both **HonKit** (build a static site) and **GitBook** (Git Sync).

This file is not published (it is not in `SUMMARY.md` and is listed in `.bookignore`).

## Preview locally

```bash
npm install
npm run serve     # http://localhost:4000, reloads on save
npm run build     # static site in _book/
```

## Layout

```
.
├── README.md            # docs home
├── SUMMARY.md           # the sidebar. A page not listed here is invisible
├── book.json            # HonKit config
├── .gitbook.yaml        # GitBook Git Sync config
├── .gitbook/assets/     # ALL images live here
├── app/                 # merchant guide
│   ├── README.md        # Overview
│   ├── quickstart.md
│   ├── setup/           # one task per page, numbered steps
│   ├── guides/          # day-to-day work, end to end
│   └── reference/       # lookup tables + FAQ
└── mcp/                 # AI connector
```

| Folder | Answers | Written as |
| --- | --- | --- |
| `setup/` | "how do I do this specific thing" | Numbered steps, one task per page |
| `guides/` | "how do I do my daily work" | Short sections, worked routines |
| `reference/` | "what exactly does X do" | Tables. Scannable |

## Rules that keep both HonKit and GitBook working

1. **No GitBook-only blocks.** Don't use `{% hint %}`, `{% tabs %}` or `{% code %}`; HonKit fails
   on them. Use a blockquote for callouts: `> **Tip.** …`
2. **Never type double curly braces as-is.** HonKit treats them as template tags and the text
   disappears. For email variables write
   `<code>&#123;&#123;cart_id&#125;&#125;</code>` (see `app/reference/email-variables.md`).
3. **Quote UI labels exactly** as they appear in the English app, in bold: **Save Template**.
4. **Relative links** to `.md` files: `[Plan features](../reference/plan-features.md)`.
5. **Images** go in `.gitbook/assets/` and are linked relatively:
   `![Dashboard tabs](../../.gitbook/assets/dashboard-tabs.png)`.

## Adding a page

1. Create the `.md` file in the right folder, with front matter:
   ```yaml
   ---
   description: One sentence. Shows in search results.
   ---
   ```
2. Add it to `SUMMARY.md` where it should appear.
3. Run `npm run build` and check it finishes without errors.
4. Commit and push.

## Screenshots still to take

The pages have no screenshots yet. Suggested shots, in `.gitbook/assets/`:

| File | Page | Shot |
| --- | --- | --- |
| `home-setup-guide.png` | quickstart | Home with the Setup Guide |
| `theme-app-embed.png` | setup/enable-app-embed | Theme editor, App embeds, Cb Customer Cart Widget on |
| `storefront-widget.png` | setup/enable-app-embed | Cart page showing "Your Cart ID" |
| `widget-templates.png` | setup/widget-templates | Choose Widget Template page |
| `custom-template-builder.png` | setup/widget-templates | Design Custom Template with Live Preview |
| `widget-visibility.png` | setup/widget-visibility | Settings → Widget Visibility |
| `support-form.png` | setup/popup-and-support-form | Form Fields editor, and the storefront Contact Support window |
| `email-merchant-alerts.png` | setup/email-notifications | Merchant Alerts tab |
| `dashboard-tabs.png` | guides/dashboard | Dashboard stat cards and tabs |
| `cart-detail.png` | guides/review-a-cart | Cart page with items, feed and customer |
| `draft-builder.png` | guides/draft-orders | Build Draft Order page |
| `analytics.png` | guides/analytics | Analytics with date picker |
| `plan-usage.png` | guides/plans-and-billing | Home → Plan Usage & Caps |
| `mcp-token.png` | mcp/setup | Create an access token, and the one-time token banner |

## Before publishing

Confirm with the team, because these can be changed from the internal admin panel and the docs use
the code defaults:

- Plan prices and trial length (`app/guides/plans-and-billing.md`, `app/reference/plan-features.md`)
- Monthly limits, retention days and MCP rate limits (`app/reference/plan-features.md`)
- Whether MCP is available on Free
