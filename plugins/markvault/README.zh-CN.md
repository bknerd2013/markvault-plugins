# MarkVault · 拾页

[English](README.md) | 简体中文

1. 在拾页设置中，将命令行授权文件导出到 `~/.markvault/entitlement.jwt`。试用期和有效的付费授权均可使用。
2. [安装插件](../../README.zh-CN.md)，然后新建对话。
3. 告诉模型归档目录的位置，可在设置的**数据位置**中找到。模型会调用 `connect_archive`，连接并记住这个目录。

Claude Code 需要 Node.js 20 或更高版本；Codex 自带 Node 运行环境。归档保留在本机，只有你提出要求时才会写入概览图表。替换授权文件后，下次调用即会生效。

## 在概览页生成图表

复制下面的提示词：

```text
请使用 MarkVault MCP 分析我的 X 收藏。先用 search_bookmarks 抽样查看不同时期的内容，识别 6 到 10 个主题，并列出每个主题的关键词。再用 count_bookmarks 按月统计各主题的命中数，同时告诉我没有命中任何主题的收藏占比。最后用 write_overview_block 写回三个概览区块：主题分布，id 为 theme-share，使用 bars；各主题的占比随时间变化，id 为 theme-trend，使用 lines，unit 为 percent；主题与年份的交叉表，id 为 theme-by-year，使用 table，matrix 为 true，主题作为行、年份作为列，unit 为 percent。在 method 中说明使用了多少组关键词，以及如何匹配。
```

打开拾页的概览页即可查看图表。再次使用相同提示词，会更新同名区块。
