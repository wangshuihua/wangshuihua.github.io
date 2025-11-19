---
layout: page
title: Logs
---
{% for post in site.posts %}
{% if post.layout == 'log' %}
<div class="logs">
  <h2 class="">{{ post.title }}</h2>
  {% if post.image %}
    <div class="thumbnail-container" style="background-image:url({{ site.github.url}}{{ post.image}});">
  </div>
  {% endif %}
  <p>
    {{ post.content }}
    <span class="post-date"><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date_to_string }} -
      <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span>
  </p>
</div>
{% endif %}
{% endfor %}