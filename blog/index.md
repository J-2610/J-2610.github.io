---
title: 博客
---
{% include header.html %}

<div class="page-content">
  <div class="page-content__inner">

    <h1>📝 博客</h1>
    <p>学习笔记与踩坑记录（持续更新中）</p>

    {% for post in site.posts %}
      <div style="border-bottom:1px solid #e0e0e0; padding:16px 0;">
        <h2 style="margin-bottom:8px;">
          <a href="{{ post.url }}">{{ post.title }}</a>
        </h2>
        <p class="post-meta" style="color:#888; font-size:0.9em; margin-top:0;">
          📅 {{ post.date | date: "%Y-%m-%d" }}
        </p>
        <p>{{ post.excerpt | truncatewords: 80 }}</p>
      </div>
    {% endfor %}

  </div>
</div>
