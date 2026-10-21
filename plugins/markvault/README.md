# MarkVault

English | [简体中文](README.zh-CN.md)

1. Open **Connect AI tools** in MarkVault Settings and confirm step 1 is ready. The access file is prepared automatically and saved inside your bookmark folder. A trial or active paid licence is required.
2. Click **Copy repository URL** in the card, add the marketplace in your desktop app using the path below, then install `markvault`.
3. Start a new conversation and say: **“Please connect my MarkVault library and count my saved bookmarks.”** It finds your archive automatically; if several are found, choose one.

Repository URL: `https://github.com/bknerd2013/markvault-plugins`

- **Claude**: Customize → Plugins → Add → Add marketplace → Add from a repository → paste URL and choose **Use “…”** → Sync → Discover → click Add on Markvault.
- **Codex**: Plugins → ⚙ → Add → Add a marketplace → paste URL into Source → Add marketplace → Personal → click + on MarkVault to install markvault.

See the [illustrated guide](https://markvault.app/guide/ai-tools/).

The repository’s [setup screenshots](../../README.md#setup-screenshots) cover both apps: menus, repository dialogs, plugin lists, installed states, first tool approvals, and demo replies.

![MarkVault Connect AI tools card](https://markvault.app/img/guide/step1-card-gui-localized-en.webp)

Claude’s local plugin needs Node.js 20 or later; Codex supplies its own Node runtime. Your saved archive stays on your computer. The plugin only writes charts when asked; automatically refreshed access takes effect on the next call.

## Add charts to Overview

```text
Use MarkVault MCP to analyze my X bookmarks. First use search_bookmarks to sample content from different periods, identify 6 to 10 themes, and list keywords for each theme. Then use count_bookmarks to count each theme's hits by month, and also tell me the share that matched no theme. If more than 10% matched no theme, call count_bookmarks again with unmatched_sample set to 30, read those posts, add keywords or a new theme for what they have in common, and count once more; do this at most once. Finally, use write_overview_block to write back three blocks: a theme distribution with id theme-share (bars), each theme's share over time with id theme-trend (lines, unit percent), and a themes × years cross-tab with id theme-by-year (table with matrix true, themes as rows and years as columns, unit percent). In the method field, state how many keyword groups you used and how they were matched.
```

Open MarkVault's Overview page to see the charts. Repeating the prompt updates the same blocks.

## Update an installed plugin

Start by checking for updates in the desktop app, keeping the existing plugin and marketplace in place.

### Claude: check for updates

Customize → Plugins → Yours → Markvault → ⋯ → Check for updates → Update

Open the installed Markvault plugin, choose Check for updates from its ⋯ menu, then click Update when an update is available. If the page keeps showing the previous update time, quit and reopen Claude, then check the version and enabled switch again. In our check, version 1.0.4 was confirmed after restarting; the version shown before clicking Update can already be the marketplace version.

### Codex: upgrade from the marketplace

Settings → Plugins → Marketplace → markvault-plugins → Upgrade

Click Upgrade beside markvault-plugins and wait for the spinner to finish. In this verified flow, the installed plugin updates with the marketplace; there is no separate plugin-level Update step. Then open Plugins → MarkVault in Settings to check Version, and confirm that the plugin remains enabled. The “markvault-plugins marketplace upgraded” notification also appears when no new version is available; use the version number to check the result.

After an update, start a new conversation and ask MarkVault to connect to your library and count your bookmarks. Allow the tool connection if asked, then check the result against your own library; 36 is the size of our demo library, not an expected count for every user.

[Illustrated update steps](https://markvault.app/guide/ai-tools/#plugin-updates)

## Other ways: terminal (advanced)

```sh
claude plugin marketplace add bknerd2013/markvault-plugins && claude plugin install markvault@markvault-plugins
```

```sh
codex plugin marketplace add bknerd2013/markvault-plugins && codex plugin add markvault@markvault-plugins
```
