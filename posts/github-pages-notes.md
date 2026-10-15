---
layout: post
title: "用 GitHub Pages 搭建个人主页踩坑记录"
date: 2026-07-17
tags: [GitHub, Pages, Jekyll]
---

记录一下用 GitHub Pages 搭建个人主页的全过程。

## 环境

- 仓库：`J-2610.github.io`（GitHub Pages 个人主页仓库命名规则：`用户名.github.io`）
- 主题：`jekyll-theme-calm`
- 自定义域名：`062610.cc.cd`

## 踩过的坑

### 1. 自定义域名 CNAME

在仓库根目录放一个 `CNAME` 文件，内容是域名。注意：

- 本地解析 DNS 需要去域名服务商处配置
- GitHub 会做 HTTPS 证书签发，一般等 10~30 分钟生效
- 如果域名解析了 `@`（根域名），要额外加一条 `www` 或直接用泛解析

### 2. Jekyll 主题选择

官方有 8 个内置主题，不需要安装依赖，改 `_config.yml` 里的 `theme` 一行就行。常用的：

- `jekyll-theme-minimal`：极简，内容为主
- `jekyll-theme-calm`：柔和色调，适合个人站
- `jekyll-theme-slate`：深色，科技感

### 3. Pages 构建缓存

改了 `_config.yml` 后如果页面没更新，多半是 GitHub Pages 的构建缓存。可以在仓库的 Settings → Pages 里手动触发一次重新构建，或者提交一个空 commit 触发。

## 小结

个人主页 = 一个 Jekyll 仓库，不需要后端，免费托管。
