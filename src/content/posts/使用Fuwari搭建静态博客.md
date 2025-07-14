---
title: 使用Fuwari搭建静态博客
published: 2025-07-14
description: '详细介绍如何使用Fuwari搭建现代化的静态博客，包括安装、配置、写作和部署的完整流程'
image: ''
tags: [Vercel, Astro, 静态博客, Tailwind CSS]
category: '教程'
draft: false 
lang: 'zh_CN'
---

## 🍥 Fuwari 简介

Fuwari 是一个基于 [Astro](https://astro.build) 框架构建的现代化静态博客模板。它以简洁优雅的设计和强大的功能著称，为个人博客和技术写作提供了完美的解决方案。

![Fuwari 博客预览](https://raw.githubusercontent.com/saicaca/resource/main/fuwari/home.png)

> **为什么选择 Fuwari？**  
> 相比其他静态博客方案，Fuwari 在保持简洁性的同时，提供了丰富的现代化功能，让你专注于内容创作而无需担心技术细节。

## 🚀 快速开始

### 1.Fork & Clone Fuwari

[Fuwari](https://github.com/saicaca/Fuwari)

```bash
git clone https://github.com/saicaca/Fuwari.git && cd Fuwari
```

### 2.环境要求

- Node.js 20+
- pnpm <= 9

### 3.安装依赖

```bash
cd Fuwari
pnpm install
```

### 4. 修改配置 & 推送

修改 `src/config.ts` 文件，修改博客的配置。

```bash
git add . && git commit -m "feat: add config" && git push
```


### 5. 部署
使用Vercel部署,一直点击next即可。
![Vercel部署](/src/assets/images/vercel.png)

