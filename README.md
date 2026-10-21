# MarkVault plugins

English | [简体中文](README.zh-CN.md)

Search your saved X bookmarks with the Claude or Codex desktop app, and add charts to MarkVault's Overview page. Your archive stays on your computer.

1. Open **Connect AI tools** in MarkVault Settings and confirm step 1 is ready. The access file is prepared automatically and saved inside your bookmark folder. A trial or active paid licence is required.
2. Click **Copy repository URL** in the card, add the marketplace in your desktop app using the path below, then install `markvault`.
3. Start a new conversation and say: **“Please connect my MarkVault library and count my saved bookmarks.”** It finds your archive automatically; if several are found, choose one.

Repository URL: `https://github.com/bknerd2013/markvault-plugins`

- **Claude**: Customize → Plugins → Add → Add marketplace → Add from a repository → paste URL and choose **Use “…”** → Sync → Discover → click Add on Markvault.
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

3. Open Discover and click Add on Markvault

![Open Discover and click Add on Markvault](https://markvault.app/img/guide/step2-claude-04-list-en-v3.webp)

4. Plugin installed

![Plugin installed](https://markvault.app/img/guide/step2-claude-06-installed-en-v2.webp)

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

4. Plugin installed

![Plugin installed](https://markvault.app/img/guide/step2-codex-06-installed-en-v2.webp)

5. Start a new conversation, send the first message above, and allow the tool connection

![Start a new conversation, send the first message above, and allow the tool connection](https://markvault.app/img/guide/step3-codex-02-confirm-en-v2.webp)

6. Demo reply: 36 saved bookmarks

![Demo reply: 36 saved bookmarks](https://markvault.app/img/guide/step3-codex-03-count-en-v2.webp)

## Update an installed plugin

Start by checking for updates in the desktop app, keeping the existing plugin and marketplace in place.

### Claude: check for updates

Customize → Plugins → Yours → Markvault → ⋯ → Check for updates → Update

Open the installed Markvault plugin, choose Check for updates from its ⋯ menu, then click Update when an update is available. If the page keeps showing the previous update time, quit and reopen Claude, then check the version and enabled switch again. In our check, version 1.0.4 was confirmed after restarting; the version shown before clicking Update can already be the marketplace version.

![Choose Check for updates from the installed plugin’s menu](https://markvault.app/img/guide/upgrade-claude-02-check-menu-en-v1.webp)

![Click Update when it is available](https://markvault.app/img/guide/upgrade-claude-03-available-en-v1.webp)

![After reopening Claude: version 1.0.4, enabled, with Update disabled](https://markvault.app/img/guide/upgrade-claude-05-after-restart-en-v1.webp)

### Codex: sync the marketplace and check the version

Settings → Plugins → Marketplace → markvault-plugins → Upgrade

Click Upgrade beside markvault-plugins and wait for the spinner to finish. Then open Plugins → MarkVault in Settings and check Version and the enabled switch in the plugin list. The “markvault-plugins marketplace upgraded” notification confirms a marketplace sync; it does not prove the installed plugin changed version.

In our October 21, 2026 check, MarkVault was already at the public version 1.0.4 before and after the sync. No plugin-level Update button appeared. An upgrade from an older installed version through the GitHub marketplace and a post-upgrade tool call have not yet been verified in Codex.

![Find Upgrade on the Marketplace tab in Settings](https://markvault.app/img/guide/upgrade-codex-02-marketplace-upgrade-button-en-v1.webp)

![The notification confirms that the marketplace was synced](https://markvault.app/img/guide/upgrade-codex-04-marketplace-upgraded-toast-en-v1.webp)

![Reopen MarkVault settings and check Version (1.0.4 in this check)](https://markvault.app/img/guide/upgrade-codex-05-current-version-en-v1.webp)

After an update, start a new conversation and ask MarkVault to connect to your library and count your bookmarks. Allow the tool connection if asked, then check the result against your own library; 36 is the size of our demo library, not an expected count for every user.

[Illustrated update steps](https://markvault.app/guide/ai-tools/#plugin-updates)

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
