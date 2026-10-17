# MarkVault plugins

English | [简体中文](README.zh-CN.md)

Search your saved X bookmarks with Claude Code or Codex, and add charts to MarkVault's Overview page. Your archive stays on your computer.

1. In MarkVault **Settings**, export the command-line entitlement file and save it as `~/.markvault/entitlement.jwt`. A 14-day trial or active paid licence includes MCP.
2. Install the plugin with either pair of commands below. Claude Code requires Node.js 20 or later; Codex supplies its own Node runtime.
3. Start a new conversation and say: **“My MarkVault archive folder is /path/to/my/archive. Connect it and count my saved bookmarks.”** Find your folder under **Data location** in MarkVault Settings. The plugin remembers it for future conversations.

Claude Code:

```sh
claude plugin marketplace add bknerd2013/markvault-plugins
claude plugin install markvault@markvault-plugins
```

Codex:

```sh
codex plugin marketplace add bknerd2013/markvault-plugins
codex plugin add markvault@markvault-plugins
```

See [the plugin guide](plugins/markvault/README.md) for a ready-to-use Overview prompt. MarkVault is proprietary software; see [LICENSE](LICENSE). Bundled third-party notices are in `plugins/markvault/server/THIRD_PARTY_NOTICES.txt`.
