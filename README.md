# 📝 Hexo 博客操作指南

本文档介绍如何使用 Hexo 创建、编辑博客文章、预览效果以及如何将博客部署到 GitHub Pages 上。

---

## 1. 修改或新建博客文章

### 创建新文章

首先，在终端中运行以下命令来创建一个新的博客文章：

```bash
hexo new "你的新文章标题"
```

这将在 `source/_posts/` 文件夹中生成一个 `.md` 文件，文件名为文章的创建日期和标题。你可以打开该文件并编辑文章内容。

例如：

```markdown
---
title: 新文章标题
date: 2025-07-20 18:00:00
tags: [标签1, 标签2]
cover: /img/example.png
---

这是新文章的内容～
```

编辑完成后，保存文件。

---

## 2. 本地预览查看效果

### 生成静态文件并启动本地服务

在博客目录下运行以下命令来清理缓存、生成静态文件并启动本地服务器：

```bash
hexo clean && hexo g && hexo s
```

然后，打开浏览器访问 [http://localhost:4000](http://localhost:4000)，即可看到你修改后的博客效果。

---

## 3. 部署到 GitHub 上

### 配置 GitHub 仓库

确保你已经配置好 GitHub Pages 仓库，仓库名格式为 `<你的用户名>.github.io`。

### 部署命令

在 Hexo 博客项目的根目录下，运行以下命令将生成的静态网页部署到 GitHub Pages 上：

```bash
hexo d
```

这条命令会自动将 `public/` 文件夹中的静态网页上传到你配置的 GitHub 仓库。几秒钟后，部署完成。

### 访问地址

部署完成后，你可以通过 GitHub Pages 的链接访问你的博客，地址通常为：

```
https://<你的用户名>.github.io/
```

例如，如果你的 GitHub 用户名是 `bae-ace`，那么你的博客地址将是：[https://bae-ace.github.io](https://bae-ace.github.io)。

