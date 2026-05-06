# OpenWalk 博客

> 个人主要文章发布站点，基于 AstroPaper 主题。

## 站点信息

| 项目 | 值 |
|------|-----|
| 部署域名 | https://wangyiguo.top/ |
| GitHub 仓库 | https://github.com/jeekeagle/NextBlog |
| 同步路径 | `/opt/data/obsidian/N6-Output/Output-Site/OpenWalk/sources` |
| 文章目录 | `src/data/blog/` |
| 图片目录 | `src/assets/images/` |
| 作者 | theo |
| 主题 | AstroPaper |
| 时区 | Asia/Shanghai |

## 目录结构

```
OpenWalk/                    # 本地工作目录
└── sources/                 # Git 仓库根目录（与远程同步的路径）
    ├── .git/
    ├── src/
    │   ├── assets/images/   # 文章配图
    │   ├── config.ts        # 站点配置
    │   ├── constants.ts     # 常量/链接
    │   ├── content.config.ts # Astro 内容集合配置
    │   └── pages/           # 页面路由（about.md、posts 等）
    ├── public/              # 静态资源
    ├── astro.config.ts
    ├── package.json
    └── README.md            # AstroPaper 原始说明（上游）
```

## 发布规则

- `pubDatetime` 必须使用**过去的时间**（AstroPaper 定时发布机制）
- 北京时间 5:00 = UTC 前一天 21:00
- 文章从 `h2` 开始，不使用 `h1`
- 图片使用标准 Markdown 语法
- 翻译文章必须添加 `canonicalURL`

## Skill

> 📋 完整运营指南（发文章规范、GitHub 操作、Vercel 部署）见父目录 `../readme`

- 发布文章使用 **`write-after-post-open`** skill
  - 路径：`/opt/data/obsidian/N0-Agent/skills/next-skills/write-after-post-open/`
- Flow Post 使用 **`write-after-post-flow`** skill
  - 路径：`N0-Agent/skills/next-skills/write-after-post-flow/`
