---
layout: default
title: Gallery
permalink: /media/gallery/
nav: false
---

{% include media-styles.html %}

<div class="media-archive">
  <a class="archive-back" href="{{ '/media/' | relative_url }}">← Back to Media</a>
  <h1>Gallery</h1>
  <p class="media-intro">Selected photos and moments from MORIN Lab activities and lab life</p>

  <div class="archive-grid">
    {% assign gallery_items = site.media_gallery | sort: "order" %}
    {% for item in gallery_items %}
      {% include media-gallery-card.html item=item card_class="archive-card" meta_class="archive-meta" %}
    {% endfor %}
  </div>
</div>
