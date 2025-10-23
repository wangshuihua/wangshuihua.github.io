---
layout: page
title: Inside Emotions（情绪研究室）
---

<ul class="posts">
  {% for post in site.posts %}
    {% if post.type == 'psychology' %}
      <li itemscope>
        <a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a>
        <p class="post-date"><span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%B %-d" }} - <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span></p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
