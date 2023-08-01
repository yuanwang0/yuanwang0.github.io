---
layout: page
permalink: /news/
title: NEWS
nav: true
nav_order: 1
horizontal: true
---
<!-- _pages/news.md -->
<hr>

<div class="posts">
  {% for post in site.news reversed %}
  <div class="post">
    <h5 class="post-date">{{ post.date | date: "%B %-d, %Y" }}</h5>
    {{ post.content }}
    <br>
    <hr>
  </div>
  {% endfor %}
</div>
