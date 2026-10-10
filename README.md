# Long77730 · 个人博客

一个使用 Markdown、Jekyll 和 GitHub Pages 发布的个人博客。文章保存在 `_posts/`，页面样式由原生 CSS 编写。

## 博客地址

<https://long77730.github.io/>

GitHub 个人主页：<https://github.com/Long77730>

## 新增文章

在 `_posts/` 中新增 `YYYY-MM-DD-title.md`，并使用现有 Front Matter：

```yaml
---
layout: post
title: 文章标题
date: 2026-10-10
excerpt: 一句话摘要
tags:
  - 学习
---
```

第二个 `---` 之后直接写 Markdown 正文。

## 修改网站

- `_config.yml`：网站标题、简介、链接和时区
- `index.html`：首页介绍、文章列表和项目卡片
- `about.md`：个人介绍
- `_posts/*.md`：博客文章
- `assets/style.css`：配色、排版和响应式样式
- `.github/workflows/pages.yml`：GitHub Pages 自动构建与发布

## 发布

提交并推送到 `main` 后，GitHub Actions 会运行 Jekyll 并把静态页面发布到 GitHub Pages。仓库的 Pages 发布源应设置为 **GitHub Actions**。

```text
Markdown 文章 → Jekyll / GitHub Actions → 静态 HTML → GitHub Pages
```

本地写作不需要安装 Node.js、npm、React、Vue、Ruby 或数据库。
