# MarkVault · 拾页插件

[English](README.md) | 简体中文

在 Claude 或 Codex 桌面应用中搜索你保存的 X 收藏，并把图表写回拾页的概览页。归档保留在你的电脑上。

1. 打开拾页设置中的**连接 AI 工具**，确认第 1 步已就绪。授权文件会自动准备并保存在收藏文件夹内。试用期和有效的付费授权均可使用。
2. 从卡片点击**复制仓库地址**，按下方的桌面应用路径添加 marketplace，再安装 `markvault`。
3. 新建对话，说一句：**“请连接我的拾页库并统计收藏数。”** AI 会自动寻找收藏库；若找到多个，请选择你使用的那个。

仓库地址：`https://github.com/bknerd2013/markvault-plugins`

- **Claude**：自定义 → 插件 → 添加 → 添加市场 → 从仓库添加 → 粘贴地址并选择 **使用“…”** → 同步 → 发现 → 点 Markvault 的 + 添加插件。
- **Codex**：插件 → ⚙ → 添加 → 添加插件市场 → 粘贴地址到「来源」 → 添加市场 → 个人 → 点 MarkVault 的 + 安装插件。

完整步骤见[图文指南](https://markvault.app/zh/guide/ai-tools/)。

<a id="setup-screenshots"></a>

## 安装步骤配图

截图使用简体中文界面、中文提问和中文回复。工具名称、插件自带说明和应用尚未翻译的提示保留原文。36 条是演示库的当前收藏数；你的回复会显示自己的收藏数。

### 1. 在拾页中复制仓库地址

![授权文件已就绪，复制仓库地址](https://markvault.app/img/guide/step1-card-gui-localized-zh.webp)

### Claude

1. 打开“添加”菜单

![打开“添加”菜单](https://markvault.app/img/guide/step2-claude-01-menu-zh-v2.webp)

2. 填入地址，选择“使用”并点击“同步”

![填入地址，选择“使用”并点击“同步”](https://markvault.app/img/guide/step2-claude-03-url-zh-v2.webp)

3. 在“发现”的“新插件”中找到 Markvault

![在“发现”的“新插件”中找到 Markvault](https://markvault.app/img/guide/step2-claude-04-list-zh-v2.webp)

4. 插件安装完成

![插件安装完成](https://markvault.app/img/guide/step2-claude-06-installed-zh-v2.webp)

5. 新建对话，发送上方第一句话，同意工具连接

![新建对话，发送上方第一句话，同意工具连接](https://markvault.app/img/guide/step3-claude-02-confirm-zh-v2.webp)

6. 演示库回复：36 条当前收藏

![演示库回复：36 条当前收藏](https://markvault.app/img/guide/step3-claude-03-count-zh-v2.webp)

### Codex

1. 打开“添加”菜单

![打开“添加”菜单](https://markvault.app/img/guide/step2-codex-01-menu-zh-v2.webp)

2. 在“来源”填入地址并点击“添加市场”

![在“来源”填入地址并点击“添加市场”](https://markvault.app/img/guide/step2-codex-03-url-zh-v2.webp)

3. 在“个人”页签找到 MarkVault

![在“个人”页签找到 MarkVault](https://markvault.app/img/guide/step2-codex-04-list-zh-v2.webp)

4. 插件安装完成

![插件安装完成](https://markvault.app/img/guide/step2-codex-06-installed-zh-v2.webp)

5. 新建对话，发送上方第一句话，同意工具连接

![新建对话，发送上方第一句话，同意工具连接](https://markvault.app/img/guide/step3-codex-02-confirm-zh-v2.webp)

6. 演示库回复：36 条当前收藏

![演示库回复：36 条当前收藏](https://markvault.app/img/guide/step3-codex-03-count-zh-v2.webp)

## 更新已安装的插件

先在桌面应用里检查更新，保留现有插件和市场。

### Claude：检查插件更新

自定义 → 插件 → 我的 → Markvault → ⋯ → 检查更新 → 更新

打开已安装的 Markvault，在 ⋯ 菜单中选择「检查更新」，有可用更新时点击「更新」。如果页面仍显示旧的更新时间，退出并重新打开 Claude，再核对版本和启用开关。本次在重启后确认版本为 1.0.4；点击「更新」之前，页面显示的版本也可能已经是市场版本。

![在已安装插件的菜单中选择「检查更新」](https://markvault.app/img/guide/upgrade-claude-02-check-menu-zh-v1.webp)

![有可用更新时点击「更新」](https://markvault.app/img/guide/upgrade-claude-03-available-zh-v1.webp)

![重新打开 Claude 后：版本 1.0.4、已启用，「更新」按钮不可点](https://markvault.app/img/guide/upgrade-claude-05-after-restart-zh-v1.webp)

### Codex：同步市场并核对版本

设置 → 插件 → 市场 → markvault-plugins → 升级

点击 markvault-plugins 旁的「升级」，等待按钮停止转圈。然后在设置的「插件 → MarkVault」中查看「版本」，并在插件列表核对启用开关。「markvault-plugins 市场已升级」只表示市场同步完成，不能证明已安装的插件更换了版本。

2026 年 10 月 21 日核对时，同步前后均为公开最新版 1.0.4，界面未出现插件级「更新」按钮。Codex 从旧版升级及升级后的工具调用仍待验证。

![在设置的「市场」页签找到「升级」](https://markvault.app/img/guide/upgrade-codex-02-marketplace-upgrade-button-zh-v1.webp)

![提示只确认市场已同步](https://markvault.app/img/guide/upgrade-codex-04-marketplace-upgraded-toast-zh-v1.webp)

![重新打开 MarkVault 设置核对版本，本次仍为 1.0.4](https://markvault.app/img/guide/upgrade-codex-05-current-version-zh-v1.webp)

更新后新建对话，请 MarkVault 连接收藏库并统计收藏数；出现工具连接确认时同意，再与自己的收藏库核对。36 条是演示库的数量，不是每位用户都应得到的结果。

[更新步骤配图](https://markvault.app/zh/guide/ai-tools/#plugin-updates)

## 其他方式：终端（高级）

Claude Code：

```sh
claude plugin marketplace add bknerd2013/markvault-plugins && claude plugin install markvault@markvault-plugins
```

Codex：

```sh
codex plugin marketplace add bknerd2013/markvault-plugins && codex plugin add markvault@markvault-plugins
```

想在概览页生成图表，可直接使用[插件使用说明](plugins/markvault/README.zh-CN.md)中的提示词。

MarkVault 为专有软件，详见 [LICENSE](LICENSE)。随附组件的第三方许可声明见 `plugins/markvault/server/THIRD_PARTY_NOTICES.txt`。
