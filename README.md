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

1. **Before checking, open the installed Markvault plugin and note its version** The screenshot shows 1.0.4 from the official markvault-plugins marketplace.

   ![Before checking: version 1.0.4 from the official markvault-plugins marketplace](https://markvault.app/img/guide/upgrade-claude-106-01-before-1.0.4-en-v1.webp)

2. **Choose Check for updates from the plugin’s ⋯ menu**

   ![Choose Check for updates from the installed plugin’s menu](https://markvault.app/img/guide/upgrade-claude-106-02-check-menu-en-v1.webp)

3. **Click Update when it becomes available** In this check, the page still showed 1.0.4 before clicking Update.

   ![Click Update when it becomes available; this page still shows 1.0.4](https://markvault.app/img/guide/upgrade-claude-106-03-available-en-v1.webp)

4. **Check the version and enabled switch; if the update time is still old, quit and reopen Claude, then check again** On October 22, 2026, we verified an in-place upgrade from 1.0.4 to 1.0.6. After reopening Claude, 1.0.6 remained enabled and Update was disabled.

   ![After reopening Claude: version 1.0.6, enabled, with Update disabled](https://markvault.app/img/guide/upgrade-claude-106-07-after-restart-1.0.6-en-v1.webp)

### Codex: upgrade from the marketplace

Settings → Plugins → Marketplace → markvault-plugins → Upgrade

Click Upgrade beside markvault-plugins and wait for the spinner to finish. In this verified flow, the installed plugin updates with the marketplace; there is no separate plugin-level Update step. Then open Plugins → MarkVault in Settings to check Version, and confirm that the plugin remains enabled. The “markvault-plugins marketplace upgraded” notification also appears when no new version is available; use the version number to check the result.

![Before upgrading: version 1.0.4 from the official markvault-plugins marketplace](https://markvault.app/img/guide/upgrade-codex-105-01-before-version-1.0.4-en-v1.webp)

![Click Upgrade beside markvault-plugins in Settings → Plugins → Marketplace](https://markvault.app/img/guide/upgrade-codex-105-02-marketplace-upgrade-button-en-v1.webp)

![After upgrading: version 1.0.5 from the same official marketplace](https://markvault.app/img/guide/upgrade-codex-105-05-updated-version-1.0.5-en-v1.webp)

![Re-check after upgrading: the same notification appears even when the version stays at 1.0.5](https://markvault.app/img/guide/upgrade-codex-105-06-recheck-toast-en-v1.webp)

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
