# MarkVault

English | [简体中文](README.zh-CN.md)

1. Open **Connect AI tools** in MarkVault Settings and confirm step 1 is ready. The access file is prepared automatically and saved inside your bookmark folder. A trial or active paid licence is required.
2. Click **Copy repository URL** in the card, add the marketplace in your desktop app using the path below, then install `markvault`.
3. Start a new conversation and say: **“Please connect my MarkVault library and count my saved bookmarks.”** It finds your archive automatically; if several are found, choose one.

Repository URL: `https://github.com/bknerd2013/markvault-plugins`

- **Claude**: Customize → Plugins → Add → Add marketplace → Add from a repository → paste URL and choose **Use “…”** → Sync → click Add on Markvault.
- **Codex**: Plugins → ⚙ → Add → Add a marketplace → paste URL into Source → Add marketplace → Personal → click + on MarkVault to install markvault.

See the [illustrated guide](https://markvault.app/guide/ai-tools/).

The repository’s [setup screenshots](../../README.md#setup-screenshots) cover both apps: menus, repository dialogs, plugin lists, installed states, first tool approvals, and demo replies.

![MarkVault Connect AI tools card](https://markvault.app/img/guide/step1-card-gui-localized-en.webp)

Claude’s local plugin needs Node.js 20 or later; Codex supplies its own Node runtime. Your saved archive stays on your computer. The plugin only writes charts when asked; automatically refreshed access takes effect on the next call.

## Add charts to Overview

```text
Use MarkVault MCP to analyze my X bookmarks. First use search_bookmarks to sample content from different periods, identify 6 to 10 themes, and list keywords for each theme. Then use count_bookmarks to count each theme's hits by month, and also tell me the share that matched no theme. Finally, use write_overview_block to write back three blocks: a theme distribution with id theme-share (bars), each theme's share over time with id theme-trend (lines, unit percent), and a themes × years cross-tab with id theme-by-year (table with matrix true, themes as rows and years as columns, unit percent). In the method field, state how many keyword groups you used and how they were matched.
```

Open MarkVault's Overview page to see the charts. Repeating the prompt updates the same blocks.

## Other ways: terminal (advanced)

```sh
claude plugin marketplace add bknerd2013/markvault-plugins && claude plugin install markvault@markvault-plugins
```

```sh
codex plugin marketplace add bknerd2013/markvault-plugins && codex plugin add markvault@markvault-plugins
```
