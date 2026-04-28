# OpenWalk 博客

> 个人主要文章发布站点，基于 AstroPaper 主题。

## 站点信息

| 项目 | 值 |
|------|-----|
| 部署域名 | https://wangyiguo.top/ |
| GitHub 仓库 | https://github.com/jeekeagle/NextBlog |
| 源码路径 | `/opt/data/obsidian/N6-Output/Output-Site/OpenWalk/source` |
| 文章目录 | `src/data/blog/` |
| 图片目录 | `src/assets/images/` |
| 作者 | theo |
| 主题 | AstroPaper |
| 时区 | Asia/Shanghai |

## 目录结构

```
OpenWalk/
├── readme.md       # 本文件
└── source/         # AstroPaper 源码
    ├── src/
    │   ├── assets/images/    # 文章配图
    │   ├── data/blog/        # 博客文章 (.md)
    │   ├── pages/            # 页面路由
    │   ├── config.ts         # 站点配置
    │   └── constants.ts      # 常量/链接
    ├── public/               # 静态资源
    ├── astro.config.mjs
    └── package.json
```

## 文章 Frontmatter 规范

```yaml
---
title: {标题}
author: theo
pubDatetime: {ISO8601，必须为过去时间}
slug: {url路径}
featured: false
draft: false
tags:
  - {标签1}
  - {标签2}
description: {描述}
canonicalURL: {原文链接，翻译文章必填}
---
```

## 发布规则

- `pubDatetime` 必须使用**过去的时间**（AstroPaper 定时发布机制）
- 北京时间 5:00 = UTC 前一天 21:00
- 文章从 `h2` 开始，不使用 `h1`
- 图片使用标准 Markdown 语法：`![封面](../../assets/images/{slug}/cover.jpg)`
- 翻译文章必须添加 `canonicalURL`

## Skill

发布文章使用 `write-after-post-open` skill（`/opt/data/obsidian/N0-Agent/skills/next-skills/write-after-post-open/`）
