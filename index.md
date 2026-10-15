---
title: J-2610 个人主页
---

<div class="page-content">
  <div class="page-content__inner">
    <h1>👋 你好，我是 J-2610</h1>

    <p style="font-size:1.2em; color:rgba(255,255,255,0.85);">
      一个喜欢折腾技术的人。这里有我的项目、学习笔记和日常记录。
    </p>

    <div class="glass">
      <h2>📌 快速导航</h2>
      <ul style="list-style:none; padding:0; margin:0;">
        <li style="margin:10px 0;"><a href="{{ site.baseurl }}/">关于我</a> — 自我介绍和技术栈</li>
        <li style="margin:10px 0;"><a href="{{ site.baseurl }}/projects/">项目列表</a> — 最近在做的事</li>
        <li style="margin:10px 0;"><a href="{{ site.baseurl }}/blog/">博客</a> — 文章归档</li>
      </ul>
    </div>

    <h2>🚀 最近的文章</h2>
    {% for post in site.posts limit:3 %}
      <div class="glass glass-blue">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p class="post-meta" style="font-size:0.85em; opacity:0.8;">📅 {{ post.date | date: "%Y-%m-%d" }}</p>
        <p>{{ post.excerpt | truncatewords: 40 }}</p>
      </div>
    {% endfor %}

    <div class="glass">
      <p style="margin:0;">GitHub: <a href="https://github.com/J-2610">J-2610</a> · 邮箱: <a href="mailto:2975842802@qq.com">2975842802@qq.com</a></p>
    </div>
  </div>
</div>
