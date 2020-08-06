# Vita Erotica 博客源文件

## 概述

Vita Erotica 基于 Hexo 博客引擎搭建，`src` 分支存放了用于生成静态页面的源文件，其中：

- `source/` 是博文 Markdown 文档；
- `themes/next/` 是 NexT 主题；

## 开发

若您希望为本站贡献博文，您可以按以下步骤操作。

### 准备工作

1. Fork 本仓库到自己的帐户下；
2. 克隆到本地 `git clone git@github.com:<your-username>/qxzh.github.io.git`；
3. 本仓库包含两个分支，`master` 分支用于展示静态页面，`src` 分支用于配置博客主题和撰写博文；因此需要切换到 `src` 分支开始撰写 `git checkout src`；

### 撰写博文

博文位于 `source/_posts` 目录下，用 Markdown 语言编写。每个 `<file-name>.md` 文件对应于一篇博文，它的访问链接是 `https://qxzh.github.io/<file-name>/`。

您可以就所选的主题新建一篇博文，文件名称建议选用由博文标题中的关键词组成的名词性短语（参考其他博文）。新建博文后，用 YAML 前言语法添加该博文的标题和创建日期。然后，您可以开始编写博文的摘要和正文，摘要和正文之间用 `<!--more-->` 标签分开。摘要一般为对文章内容的一至两句话的总结，会以卡片的形式展示在博客主页。若该博文为译文，您还可以选择附上原文。

总而言之，一篇完整的博文的内容如下：

```markdown
---
title: 标题
date: 1970-01-01 00:00:00
---

摘要

<!--more-->

正文
```

### 推送博文

1. 推送到自己 Fork 的仓库；
2. 向本仓库提交 Pull Request，注意选择分支为 `<your-username>/qxzh.github.io:src -> qxzh/qxzh.github.io:src`；
3. 等待 Pull Request 提交，或者（可选）申请成为本仓库的协作者，这样可以自行合并该 Pull Request；

本仓库基于 GitHub Action 搭建了持续集成系统，会在推送或合并时自动更新网页。
