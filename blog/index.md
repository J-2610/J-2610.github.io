---
title: 博客
---

<div class="page-content">
  <div class="page-content__inner">

    <h1>📝 博客</h1>
    <p>学习笔记与踩坑记录（持续更新中）</p>

    {% for post in site.posts %}
      <div class="glass glass-purple">
        <h2 style="margin-bottom:8px;">
          <a href="{{ post.url }}">{{ post.title }}</a>
        </h2>
        <p class="post-meta" style="font-size:0.85em; opacity:0.8; margin-top:0;">
          📅 {{ post.date | date: "%Y-%m-%d" }}
        </p>
        <p>{{ post.excerpt | truncatewords: 60 }}</p>
        <p><a class="glass-btn" href="{{ post.url }}">阅读全文 →</a></p>
      </div>
    {% endfor %}

  </div>
</div>
