# MarkVault · 拾页插件

[English](README.md) | 简体中文

在 Claude Code 或 Codex 中搜索你保存的 X 收藏，并把图表写回拾页的概览页。归档保留在你的电脑上。

1. 打开拾页设置中的**连接 AI 工具**，等待授权就绪。试用期和有效的付费授权均可使用。
2. 从卡片点击**复制仓库地址**，按下方的桌面应用路径添加 marketplace，再安装 `markvault`。
3. 新建对话，说一句：**“请连接我的拾页库并统计收藏数。”** AI 会自动寻找收藏库；若找到多个，请选择你使用的那个。

仓库地址：`https://github.com/bknerd2013/markvault-plugins`

- **Claude**：Customize → Plugins → Add → Add marketplace → Add from a repository → 粘贴地址并选择 **Use “…”** → Sync → 安装 markvault。
- **Codex**：Plugins → Add a marketplace → 粘贴地址 → 安装 markvault。

完整步骤见[图文指南](https://markvault.app/zh/guide/ai-tools/)。

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
