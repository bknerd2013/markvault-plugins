# MarkVault

English | [简体中文](README.zh-CN.md)

1. Open **Connect AI tools** in MarkVault Settings and wait for access to be ready. A trial or active paid licence is required.
2. Copy your tool’s install command from the card, paste it into a terminal and press Enter.
3. Start a new conversation and say: **“Please connect my MarkVault library and count my saved bookmarks.”** It finds your archive automatically; if several are found, choose one.

See the [illustrated guide](https://markvault.app/guide/ai-tools/).

Claude Code needs Node.js 20 or later; Codex supplies its own Node runtime. Your saved archive stays on your computer. The plugin only writes charts when asked; replacing your entitlement file takes effect on the next call.

## Add charts to Overview

```text
Use MarkVault MCP to analyze my X bookmarks. First use search_bookmarks to sample content from different periods, identify 6 to 10 themes, and list keywords for each theme. Then use count_bookmarks to count each theme's hits by month, and also tell me the share that matched no theme. Finally, use write_overview_block to write back three blocks: a theme distribution with id theme-share (bars), each theme's share over time with id theme-trend (lines, unit percent), and a themes × years cross-tab with id theme-by-year (table with matrix true, themes as rows and years as columns, unit percent). In the method field, state how many keyword groups you used and how they were matched.
```

Open MarkVault's Overview page to see the charts. Repeating the prompt updates the same blocks.
