---
layout: default
title: Media
permalink: /media/
nav: true
nav_order: 5
---

{% include media-styles.html %}

<div class="media-page">
  <h1>Media</h1>
  <p class="media-intro">Selected videos and photos from MORIN Lab research and activities</p>

  {% assign featured = site.media_videos | where: "featured", true | first %}
  {% if featured %}
  <section class="media-section">
    <div class="media-section-head"><h2>Featured</h2></div>
    <article class="media-featured-video">
      <div class="media-video-wrap">
        <iframe
          src="https://www.youtube.com/embed/{{ featured.youtube_id }}{% if featured.youtube_start %}?start={{ featured.youtube_start }}{% endif %}"
          title="{{ featured.title }}"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen></iframe>
      </div>
      <div class="media-featured-meta">
        <p class="media-label">Featured Video</p>
        <h3 class="media-title">{{ featured.title }}</h3>
      </div>
    </article>
  </section>
  {% endif %}

  <section class="media-section">
    <div class="media-section-head">
      <h2>Videos</h2>
      <a class="media-view-all" href="{{ '/media/videos/' | relative_url }}">View all →</a>
    </div>
    <div class="media-grid">
      {% assign videos = site.media_videos | sort: "order" %}
      {% for video in videos limit:3 %}
        {% include media-video-card.html video=video %}
      {% endfor %}
    </div>
  </section>

  <section class="media-section">
    <div class="media-section-head">
      <h2>Gallery</h2>
      <a class="media-view-all" href="{{ '/media/gallery/' | relative_url }}">View all →</a>
    </div>
    <div class="media-grid">
      {% assign gallery_items = site.media_gallery | sort: "order" %}
      {% for item in gallery_items limit:3 %}
        {% include media-gallery-card.html item=item %}
      {% endfor %}
    </div>
  </section>
</div>
