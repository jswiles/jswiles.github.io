---
layout: post
title: Blog
permalink: /blog
---
<h1><u> Posts </u> </h1>
<ul>
  {% for post in site.posts %}
  <li><a style="color:blue;" href="{{ post.url }}" class="post-preview">{{ post.title }}</a></li>
  {% endfor %}
</ul>

