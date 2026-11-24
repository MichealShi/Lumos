# Lumos Markdown

一个为 macOS 打造的 Markdown 编辑器：全语法兼容、实时预览、数学公式、流程图与代码高亮。

> 目前仅提供 macOS 版本（Apple Silicon / arm64）。

## 功能特性

- **实时分屏预览**：左侧编辑、右侧即时渲染，支持滚动同步与可拖动分隔条，可切换「编辑 / 分屏 / 预览」三种视图
- **完整 Markdown 语法**：基于 CommonMark + GFM，支持表格（含合并单元格）、任务列表（可点击勾选并回写源码）、脚注、定义列表、上/下标、删除线、高亮、emoji、自动链接等
- **扩展渲染**：KaTeX 数学公式（`$...$`、`$$...$$`、`\(...\)`、`\[...\]`）、Mermaid 图表、highlight.js 代码高亮、多种提示块（tip / note / info / warning / danger）
- **编辑体验**：CodeMirror 6 编辑器、语法高亮、明暗主题、快捷键格式化（`⌘B` / `⌘I` / `⌘K`）、字数与行号状态栏
- **文件操作**：新建 / 打开 / 保存 Markdown、导出独立 HTML、Finder 中直接用 `.md` 打开、最近文档、窗口状态记忆

## 技术栈

Electron 45 · Vite 8 · CodeMirror 6 · markdown-it 14 · KaTeX · Mermaid · highlight.js

## 本地开发

```bash
npm install
npm start          # 构建并启动
npm run build      # 仅构建渲染层
npm run dist       # 打包 macOS 应用
```

> 若从 WorkBuddy 等注入了 `ELECTRON_RUN_AS_NODE=1` 的环境启动，需先执行 `unset ELECTRON_RUN_AS_NODE`。

## 许可证

MIT
