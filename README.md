# Jieyi's Blog

基于 [Jekyll Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) 的个人博客，发布在 GitHub Pages。

## 发布一篇文章

1. 在 `_posts` 目录中新建 Markdown 文件，文件名格式为 `YYYY-MM-DD-英文短标题.md`。
2. 复制 `_drafts/post-template.md` 中的头部信息，并修改标题、日期、分类和标签。
3. 写完后提交并推送到 `main` 分支；GitHub Actions 会自动构建并发布。

示例：

```markdown
---
title: 我的第一篇文章
date: 2026-09-27 10:00:00 +0800
categories: [技术, 前端]
tags: [github-pages, jekyll]
description: 一句话介绍文章内容。
---

从这里开始写正文。
```

`categories` 建议最多写两级，例如 `[技术, 前端]`；`tags` 可以填写多个关键词。分类页、标签页、归档页和站内搜索会自动生成。

## 本地预览

需要 Ruby 3.1 或更高版本：

```bash
bundle install
bundle exec jekyll serve
```

然后访问 `http://127.0.0.1:4000`。

## 首次启用 GitHub Pages

打开仓库的 **Settings → Pages**，在 **Build and deployment** 的 Source 中选择 **GitHub Actions**。之后每次推送到 `main` 都会自动发布到 <https://sunjieyi60.github.io>。
