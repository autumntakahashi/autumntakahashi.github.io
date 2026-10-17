---
layout: page
title: Articles
permalink: /articles/
---
<ul class="post-list">
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d, %Y" }}</time>
    {% if post.summary %}<p>{{ post.summary }}</p>{% endif %}
  </li>
{% endfor %}
</ul>
