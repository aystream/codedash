# CodeDash

Claude Code 和 Codex 会话的浏览器仪表板。查看、搜索、恢复和管理您所有的 AI 编程会话。

[English](../README.md) | [Russian / Русский](README_RU.md)

## 快速开始

```bash
npx codedash-app run
```

自动在浏览器中打开 `http://localhost:3847`。

```bash
npx codedash-app run --port=4000    # 自定义端口
npx codedash-app run --no-browser   # 不自动打开浏览器
npx codedash-app list               # 在终端中列出会话
npx codedash-app stats              # 显示统计信息
```

## 功能

**会话**
- 网格和列表视图，按项目分组
- Trigram 模糊搜索会话内容和项目
- 按工具（Claude/Codex）、标签、日期范围过滤
- 星标/置顶重要会话（始终显示在最前面）
- 标签：bug、feature、research、infra、deploy、review
- GitHub 风格的活动热力图
- 每个会话的成本估算

**启动**
- 在 iTerm2、Terminal.app、Warp、Kitty、Alacritty 中恢复会话
- 自动 `cd` 到项目目录
- 复制恢复命令到剪贴板
- 终端偏好设置在会话间保存

**管理**
- 删除会话（文件 + 历史 + 环境变量）
- 批量选择和删除
- 导出对话为 Markdown
- 显示每个会话相关的 git 提交
- 自动检查更新

**主题**：Dark、Light、System

**快捷键**：`/` 搜索，`j/k` 导航，`Enter` 打开，`x` 星标，`d` 删除，`s` 选择模式，`g` 分组，`r` 刷新，`Esc` 关闭

## 工作原理

从 `~/.claude/` 和 `~/.codex/` 读取会话数据。零依赖。全部运行在 `localhost`。

## 要求

- Node.js >= 16
- 已安装 Claude Code 或 Codex CLI
- macOS / Linux / Windows

## 许可证

MIT
