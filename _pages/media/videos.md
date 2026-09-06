---
layout: default
title: Videos
permalink: /media/videos/
nav: false
---

{% include media-styles.html %}

<div class="media-archive">
  <a class="archive-back" href="{{ '/media/' | relative_url }}">← Back to Media</a>
  <h1>Videos</h1>
  <p class="media-intro">Selected videos from MORIN Lab research and activities</p>

  <div class="archive-grid">
    {% assign videos = site.media_videos | sort: "order" %}
    {% for video in videos %}
      {% include media-video-card.html video=video card_class="archive-card" meta_class="archive-meta" %}
    {% endfor %}
  </div>
</div>
