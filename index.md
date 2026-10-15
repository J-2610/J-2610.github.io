---
title: J-2610 个人主页
---

<div class="page-content">
  <div class="page-content__inner">
    <h1>👋 你好，我是 J-2610</h1>

    <p style="font-size:1.2em; color:#555;">
      一个喜欢折腾技术的人。这里有我的项目、学习笔记和日常记录。
    </p>

    <h2>📌 快速导航</h2>
    <ul>
      <li><a href="{{ site.baseurl }}/">关于我</a> — 自我介绍和技术栈</li>
      <li><a href="{{ site.baseurl }}/projects/">项目列表</a> — 最近在做的事</li>
      <li><a href="{{ site.baseurl }}/blog/">博客</a> — 文章归档</li>
    </ul>

    <h2>🚀 最近的项目</h2>
    {% for post in site.posts limit:3 %}
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="post-meta">📅 {{ post.date | date: "%Y-%m-%d" }}</p>
      <p>{{ post.excerpt | truncatewords: 50 }}</p>
      <hr>
    {% endfor %}

    <footer>
      <p>GitHub: <a href="https://github.com/J-2610">J-2610</a> · 邮箱: <a href="mailto:2975842802@qq.com">2975842802@qq.com</a></p>
    </footer>
  </div>
</div>
