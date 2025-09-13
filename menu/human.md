---
layout: page
title: The Human Manual（人的说明书）
---

<ul class="posts">
  {% for post in site.posts %}
    {% if post.type == 'human' %}
      <li itemscope>
        <a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a>
        <p class="post-date"><span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%B %-d" }} - <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span></p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
