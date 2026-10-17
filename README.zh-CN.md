# MarkVault · 拾页插件

[English](README.md) | 简体中文

在 Claude Code 或 Codex 中搜索你保存的 X 收藏，并把图表写回拾页的概览页。归档保留在你的电脑上。

1. 打开拾页的**设置**，导出命令行授权文件，保存为 `~/.markvault/entitlement.jwt`。14 天试用期和有效的付费授权均包含 MCP。
2. 按下面对应的两条命令安装插件。Claude Code 需要 Node.js 20 或更高版本；Codex 自带 Node 运行环境。
3. 新建对话，告诉模型：**“我的拾页归档目录是 /path/to/my/archive，请连接它，并统计我保存了多少条收藏。”** 目录位置可在拾页设置的**数据位置**中找到。连接成功后，插件会记住这个目录。

Claude Code：

```sh
claude plugin marketplace add bknerd2013/markvault-plugins
claude plugin install markvault@markvault-plugins
```

Codex：

```sh
codex plugin marketplace add bknerd2013/markvault-plugins
codex plugin add markvault@markvault-plugins
```

想在概览页生成图表，可直接使用[插件使用说明](plugins/markvault/README.zh-CN.md)中的提示词。

MarkVault 为专有软件，详见 [LICENSE](LICENSE)。随附组件的第三方许可声明见 `plugins/markvault/server/THIRD_PARTY_NOTICES.txt`。
