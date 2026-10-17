---
layout: page
title: Art
permalink: /art/
---
Selected work. Each piece is listed in `_data/art.yml`; drop an image into `assets/art/` and add an entry.

<div class="gallery">
{% for piece in site.data.art %}
  <figure>
    <img src="{{ piece.image | relative_url }}" alt="{{ piece.alt | default: piece.title }}" loading="lazy">
    <figcaption>
      <span class="piece-title">{{ piece.title }}</span>
      <span class="piece-detail">{{ piece.medium }}, {{ piece.year }}</span>
    </figcaption>
  </figure>
{% endfor %}
</div>
