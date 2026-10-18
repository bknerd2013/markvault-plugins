# MarkVault plugins

English | [简体中文](README.zh-CN.md)

Search your saved X bookmarks with the Claude or Codex desktop app, and add charts to MarkVault's Overview page. Your archive stays on your computer.

1. Open **Connect AI tools** in MarkVault Settings and wait for access to be ready. A trial or active paid licence is required.
2. Click **Copy repository URL** in the card, add the marketplace in your desktop app using the path below, then install `markvault`.
3. Start a new conversation and say: **“Please connect my MarkVault library and count my saved bookmarks.”** It finds your archive automatically; if several are found, choose one.

Repository URL: `https://github.com/bknerd2013/markvault-plugins`

- **Claude**: Customize → Plugins → Add → Add marketplace → Add from a repository → paste URL and choose **Use “…”** → Sync → install markvault.
- **Codex**: Plugins → ⚙ → Add → Add a marketplace → paste URL into Source → Add marketplace → Personal → click + on MarkVault to install markvault.

See the [illustrated guide](https://markvault.app/guide/ai-tools/).

<a id="setup-screenshots"></a>

## Setup screenshots

Screenshots use the English interface, English questions, and English replies. The 36-bookmark result is from a demo library; your reply will show your own count.

### 1. Copy the repository URL in MarkVault

![Access is ready: copy the repository URL](https://markvault.app/img/guide/step1-card-gui-localized-en.webp)

### Claude

1. Open the Add menu

![Open the Add menu](https://markvault.app/img/guide/step2-claude-01-menu-en-v2.webp)

2. Enter the URL, choose Use “…” and click Sync

![Enter the URL, choose Use “…” and click Sync](https://markvault.app/img/guide/step2-claude-03-url-en-v2.webp)

3. Find Markvault in the plugin list

![Find Markvault in the plugin list](https://markvault.app/img/guide/step2-claude-04-list-en-v2.webp)

4. Plugin 1.0.2 installed

![Plugin 1.0.2 installed](https://markvault.app/img/guide/step2-claude-06-installed-en-v2.webp)

5. Start a new conversation, send the first message above, and allow the tool connection

![Start a new conversation, send the first message above, and allow the tool connection](https://markvault.app/img/guide/step3-claude-02-confirm-en-v2.webp)

6. Demo reply: 36 saved bookmarks

![Demo reply: 36 saved bookmarks](https://markvault.app/img/guide/step3-claude-03-count-en-v2.webp)

### Codex

1. Open the Add menu

![Open the Add menu](https://markvault.app/img/guide/step2-codex-01-menu-en-v2.webp)

2. Enter the URL in Source and click Add marketplace

![Enter the URL in Source and click Add marketplace](https://markvault.app/img/guide/step2-codex-03-url-en-v2.webp)

3. Find MarkVault on the Personal tab

![Find MarkVault on the Personal tab](https://markvault.app/img/guide/step2-codex-04-list-en-v2.webp)

4. Plugin 1.0.2 installed

![Plugin 1.0.2 installed](https://markvault.app/img/guide/step2-codex-06-installed-en-v2.webp)

5. Start a new conversation, send the first message above, and allow the tool connection

![Start a new conversation, send the first message above, and allow the tool connection](https://markvault.app/img/guide/step3-codex-02-confirm-en-v2.webp)

6. Demo reply: 36 saved bookmarks

![Demo reply: 36 saved bookmarks](https://markvault.app/img/guide/step3-codex-03-count-en-v2.webp)

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
