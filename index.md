---
layout: default
title: Home
---
<h1>{{ site.title }}</h1>

I'm a research technician working on computational neuroscience.  I write about the things I'm figuring out along the way.


## Recent articles

<ul class="post-list">
{% for post in site.posts limit:3 %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d, %Y" }}</time>
  </li>
{% endfor %}
</ul>

[All articles]({{ '/articles/' | relative_url }})
