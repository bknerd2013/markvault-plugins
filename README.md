# MarkVault plugins

English | [简体中文](README.zh-CN.md)

Search your saved X bookmarks with Claude Code or Codex, and add charts to MarkVault's Overview page. Your archive stays on your computer.

1. Open **Connect AI tools** in MarkVault Settings and wait for access to be ready. A trial or active paid licence is required.
2. Copy your tool’s install command from the card, paste it into a terminal and press Enter.
3. Start a new conversation and say: **“Please connect my MarkVault library and count my saved bookmarks.”** It finds your archive automatically; if several are found, choose one.

See the [illustrated guide](https://markvault.app/guide/ai-tools/).

Claude Code:

```sh
claude plugin marketplace add bknerd2013/markvault-plugins && claude plugin install markvault@markvault-plugins
```

Codex:

```sh
codex plugin marketplace add bknerd2013/markvault-plugins && codex plugin add markvault@markvault-plugins
```

See [the plugin guide](plugins/markvault/README.md) for a ready-to-use Overview prompt. MarkVault is proprietary software; see [LICENSE](LICENSE). Bundled third-party notices are in `plugins/markvault/server/THIRD_PARTY_NOTICES.txt`.
