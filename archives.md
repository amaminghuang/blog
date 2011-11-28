---
layout:           default
title:            Archives
---
<article id="post-list">
  <h3>{{ page.title }}<span>(&nbsp;{{ site.posts | size }} posts.&nbsp;)</span></h3>
  <ul class="posts">
    {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span>&nbsp;&raquo;&nbsp;<a href="/{{ post.url }}" title="{{ post.title }}" alt="bookmark">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</article>

