---
layout: page
title: Research
permalink: /research/
---
A short paragraph on my research interests goes here. Then the list below is generated from `_data/publications.yml`, so adding a paper means adding a few lines to that file.

{% for pub in site.data.publications %}
<div class="pub">
  <p class="pub-title">{{ pub.title }}</p>
  <p class="pub-authors">{{ pub.authors }}</p>
  <p class="pub-venue">{{ pub.venue }}, {{ pub.year }}</p>
  {% if pub.links %}
  <p class="pub-links">
    {% for link in pub.links %}<a href="{{ link.url }}">{{ link.label }}</a>{% endfor %}
  </p>
  {% endif %}
</div>
{% endfor %}
