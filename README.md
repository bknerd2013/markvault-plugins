# MarkVault plugins

English | [简体中文](README.zh-CN.md)

Search your saved X bookmarks with Claude Code or Codex, and add charts to MarkVault's Overview page. Your archive stays on your computer.

1. Open **Connect AI tools** in MarkVault Settings and wait for access to be ready. A trial or active paid licence is required.
2. Click **Copy repository URL** in the card, add the marketplace in your desktop app using the path below, then install `markvault`.
3. Start a new conversation and say: **“Please connect my MarkVault library and count my saved bookmarks.”** It finds your archive automatically; if several are found, choose one.

Repository URL: `https://github.com/bknerd2013/markvault-plugins`

- **Claude**: Customize → Plugins → Add → Add marketplace → Add from a repository → paste URL and choose **Use “…”** → Sync → install markvault.
- **Codex**: Plugins → ⚙ → Add → Add a marketplace → paste URL into Source → Add marketplace → Personal → click + on MarkVault to install markvault.

See the [illustrated guide](https://markvault.app/guide/ai-tools/).

## Other ways: terminal (advanced)

Claude Code:

```sh
claude plugin marketplace add bknerd2013/markvault-plugins && claude plugin install markvault@markvault-plugins
```

Codex:

```sh
codex plugin marketplace add bknerd2013/markvault-plugins && codex plugin add markvault@markvault-plugins
```

See [the plugin guide](plugins/markvault/README.md) for a ready-to-use Overview prompt. MarkVault is proprietary software; see [LICENSE](LICENSE). Bundled third-party notices are in `plugins/markvault/server/THIRD_PARTY_NOTICES.txt`.
