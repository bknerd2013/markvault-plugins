# MarkVault · 拾页

[English](README.md) | 简体中文

1. 打开拾页设置中的**连接 AI 工具**，确认第 1 步已就绪。授权文件会自动准备并保存在收藏文件夹内。试用期和有效的付费授权均可使用。
2. 从卡片点击**复制仓库地址**，按下方的桌面应用路径添加 marketplace，再安装 `markvault`。
3. 新建对话，说一句：**“请连接我的拾页库并统计收藏数。”** AI 会自动寻找收藏库；若找到多个，请选择你使用的那个。

仓库地址：`https://github.com/bknerd2013/markvault-plugins`

- **Claude**：自定义 → 插件 → 添加 → 添加市场 → 从仓库添加 → 粘贴地址并选择 **使用“…”** → 同步 → 发现 → 点 Markvault 的 + 添加插件。
- **Codex**：插件 → ⚙ → 添加 → 添加插件市场 → 粘贴地址到「来源」 → 添加市场 → 个人 → 点 MarkVault 的 + 安装插件。

完整步骤见[图文指南](https://markvault.app/zh/guide/ai-tools/)。

仓库内的[安装步骤配图](../../README.zh-CN.md#setup-screenshots)包括两家应用的菜单、地址对话框、插件列表、安装完成态、首次工具确认和演示库回复。

![拾页连接 AI 工具卡片](https://markvault.app/img/guide/step1-card-gui-localized-zh.webp)

Claude 的本地插件需要 Node.js 20 或更高版本；Codex 自带 Node 运行环境。归档保留在本机，只有你提出要求时才会写入概览图表。自动更新的授权会在下次调用时生效。

## 在概览页生成图表

复制下面的提示词：

```text
请使用 MarkVault MCP 分析我的 X 收藏。先用 search_bookmarks 抽样查看不同时期的内容，识别 6 到 10 个主题，并列出每个主题的关键词。再用 count_bookmarks 按月统计各主题的命中数，同时告诉我没有命中任何主题的收藏占比。如果未命中超过两成，再调用一次 count_bookmarks 并把 unmatched_sample 设为 30，查看这些没有归入任何主题的收藏，为它们的共同内容补充关键词或新增主题后重新统计，最多补一轮。最后用 write_overview_block 写回三个概览区块：主题分布，id 为 theme-share，使用 bars；各主题的占比随时间变化，id 为 theme-trend，使用 lines，unit 为 percent；主题与年份的交叉表，id 为 theme-by-year，使用 table，matrix 为 true，主题作为行、年份作为列，unit 为 percent。在 method 中说明使用了多少组关键词，以及如何匹配。
```

打开拾页的概览页即可查看图表。再次使用相同提示词，会更新同名区块。

## 更新已安装的插件

先在桌面应用里检查更新，保留现有插件和市场。

### Claude：检查插件更新

自定义 → 插件 → 我的 → Markvault → ⋯ → 检查更新 → 更新

打开已安装的 Markvault，在 ⋯ 菜单中选择「检查更新」，有可用更新时点击「更新」。如果页面仍显示旧的更新时间，退出并重新打开 Claude，再核对版本和启用开关。本次在重启后确认版本为 1.0.4；点击「更新」之前，页面显示的版本也可能已经是市场版本。

### Codex：同步市场并核对版本

设置 → 插件 → 市场 → markvault-plugins → 升级

点击 markvault-plugins 旁的「升级」，等待按钮停止转圈。然后在设置的「插件 → MarkVault」中查看「版本」，并在插件列表核对启用开关。「markvault-plugins 市场已升级」只表示市场同步完成，不能证明已安装的插件更换了版本。

2026 年 10 月 21 日核对时，同步前后均为公开最新版 1.0.4，界面未出现插件级「更新」按钮。Codex 从旧版升级及升级后的工具调用仍待验证。

更新后新建对话，请 MarkVault 连接收藏库并统计收藏数；出现工具连接确认时同意，再与自己的收藏库核对。36 条是演示库的数量，不是每位用户都应得到的结果。

[更新步骤配图](https://markvault.app/zh/guide/ai-tools/#plugin-updates)

## 其他方式：终端（高级）

```sh
claude plugin marketplace add bknerd2013/markvault-plugins && claude plugin install markvault@markvault-plugins
```

```sh
codex plugin marketplace add bknerd2013/markvault-plugins && codex plugin add markvault@markvault-plugins
```
