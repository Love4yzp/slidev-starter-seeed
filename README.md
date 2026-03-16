# Slidev Starter Seeed

AI 驱动的演示文稿创作工具 — 基于 [Slidev](https://sli.dev) + Seeed Studio 品牌主题。

## 快速开始

```bash
git clone --recursive https://github.com/seeed-studio/slidev-starter-seeed.git
cd slidev-starter-seeed
pnpm install
pnpm dev
```

## 用 AI 创作

用 [Claude Code](https://claude.ai/claude-code)、Cursor 等 AI 工具打开项目，直接描述你想要的内容：

- 「帮我做一个产品发布的 slide，主题是 xxx」
- 「把第 3 页改成左右两栏布局，左边文字右边图片」
- 「帮我生成一张架构图，用 Mermaid」

AI 会参考 `AGENTS.md` 中的品牌规范，自动生成符合 Seeed 风格的幻灯片。

## 添加图片

1. 把图片放入 `assets/` 目录
2. 在 slides.md 中引用：`![描述](./assets/your-image.png)`
3. 或让 AI 帮你生成 Mermaid 图表

## 导出

```bash
pnpm export     # 导出 PDF
pnpm build      # 导出 SPA 网页
```

## 主题

本项目使用 [slidev-theme-seeed](https://github.com/seeed-studio/slidev-theme-seeed) 主题（以 git submodule 形式引入）。

## License

MIT
