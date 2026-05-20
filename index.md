---
layout: default
title: Daily Feeds Blog
---

# 📚 欢迎来到 Daily Feeds Blog

这是我的每日待办事项、学习笔记和技术随笔。

## 🎮 小游戏

- [🐍 贪吃蛇游戏]({{ '/snake.html' | relative_url }}) — 经典贪吃蛇，可以在网页上玩。

## 📝 最新文章

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
      &middot;
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
