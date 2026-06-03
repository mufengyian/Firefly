---
title: Firefly 一款清新美观的 Astro 博客主题模板
pubDate: 1970-01-02
pinned: true
description: Firefly 是一款基于 Astro 框架和 Fuwari 模板开发的清新美观且现代化个人博客主题模板，专为技术爱好者和内容创作者设计。该主题融合了现代 Web 技术栈，提供了丰富的功能模块和高度可定制的界面，让您能够轻松打造出专业且美观的个人博客网站。
tags: [Markdown, Firefly, 博客, 主题, 模板]
category: 文章示例
draft: false
image: ./images/firefly2.avif
---

## 🌟 项目概述

**Firefly** 是一款基于 Astro 框架和 Fuwari 模板开发的清新美观且现代化个人博客主题模板，专为技术爱好者和内容创作者设计。该主题融合了现代 Web 技术栈，提供了丰富的功能模块和高度可定制的界面，让您能够轻松打造出专业且美观的个人博客网站。


**🖥️在线预览： [Firefly - Demo site](https://firefly.cuteleaf.cn/)**

**🏠我的博客： [https://blog.cuteleaf.cn](https://blog.cuteleaf.cn/)**

**📝Firefly使用文档： [https://docs-firefly.cuteleaf.cn](https://docs-firefly.cuteleaf.cn/)**

**⭐Firefly开源地址：[https://github.com/CuteLeaf/Firefly](https://github.com/CuteLeaf/Firefly)** 

**⭐Fuwari开源地址：[https://github.com/saicaca/fuwari](https://github.com/saicaca/fuwari)**

::github{repo="CuteLeaf/Firefly"}

::github{repo="saicaca/fuwari"}

![Firefly](./images/1.avif)


## 🚀 技术架构

- **静态站点生成**: 基于 Astro ，提供极快的加载速度和优秀的 SEO 优化
- **TypeScript 支持**: 完整的类型安全，提升开发体验和代码质量
- **响应式设计**: 使用 Tailwind CSS 构建，完美适配桌面端和移动端
- **组件化开发**: 支持 Astro、Svelte 组件，灵活可扩展


## 📖 配置说明

> 📚 **详细配置文档**: 查看 [Firefly使用文档](https://docs-firefly.cuteleaf.cn/) 获取完整的配置指南

### 文章发布时间（published / pubDate）

每篇文章需要指定发布时间，支持两种字段名：

- **`published`** — 传统字段名，向后兼容
- **`pubDate`** — 新增别名，与 RSS 标准一致

两者**二选一**即可。如果同时设置，**`pubDate` 优先**。

```yaml
---
title: 我的第一篇文章
pubDate: 2026-06-15   # 到 6 月 15 日才会出现在首页
---
```

### 定时发布

发布日期设为未来时间，文章不会立即出现在首页、归档、标签、分类、RSS 或相关推荐中。只有 rebuild 时日期已到的文章才会公开可见。

配合 CI/CD 每日自动构建，即可实现定时发布，无需额外配置。