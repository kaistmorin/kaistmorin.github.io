---
layout: default
title: Media
permalink: /media/
nav: true
nav_order: 5
---

<style>
.media-page{
  --morin-navy:#0b2d5c;
  --morin-text:#1f2937;
  --morin-muted:#667085;
  --morin-line:#e6ebf0;
  width:calc(100% - 48px);
  max-width:1120px;
  box-sizing:border-box;
  margin:0 auto;
  padding:11px 0 72px;
  font-family:inherit;
}
.media-page h1{margin:0 0 12px;font-size:2.25rem;font-weight:400;line-height:1.15}
.media-intro{max-width:860px;margin:0 0 30px;color:var(--morin-text);font-size:1rem;line-height:1.55}
.media-section{margin-top:34px}
.media-section-head{display:flex;align-items:center;gap:14px;margin:0 0 15px}
.media-section-head h2{margin:0;color:var(--morin-navy);font-size:1.25rem;font-weight:600}
.media-section-head::after{content:"";flex:1;height:1px;background:var(--morin-line)}
.media-view-all{margin-left:auto;color:var(--morin-navy);font-size:.86rem;font-weight:600;text-decoration:none;white-space:nowrap}
.media-view-all:hover{text-decoration:underline}
.media-featured-video,.media-card{overflow:hidden;border:1px solid var(--morin-line);border-radius:8px;background:#fff}
.media-video-wrap{position:relative;width:100%;aspect-ratio:16/9;background:#000}
.media-video-wrap iframe{position:absolute;inset:0;width:100%;height:100%;border:0}
.media-featured-meta,.media-card-meta{padding:12px 13px 14px}
.media-label{margin:0 0 5px;color:var(--morin-muted);font-size:.78rem}
.media-title{margin:0;color:var(--morin-navy);font-size:1rem;font-weight:600;line-height:1.4}
.media-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:18px}
.media-card a{display:block;color:inherit;text-decoration:none}
.media-card a:hover .media-title{text-decoration:underline;text-underline-offset:2px}
.media-thumb{position:relative;overflow:hidden;aspect-ratio:16/9;background:#f3f5f7}
.media-thumb img{display:block;width:100%;height:100%;object-fit:cover}
.media-play::after{content:"▶";position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);width:42px;height:42px;display:grid;place-items:center;padding-left:3px;border-radius:50%;background:rgba(11,45,92,.88);color:#fff;font-size:15px}
@media(max-width:850px){.media-grid{grid-template-columns:repeat(2,minmax(0,1fr))}}
@media(max-width:640px){.media-page{width:calc(100% - 30px)}.media-grid{grid-template-columns:1fr}}
</style>

<div class="media-page">
  <h1>Media</h1>
  <p class="media-intro">Selected videos and photos from MORIN Lab research and activities</p>

  <section class="media-section">
    <div class="media-section-head"><h2>Featured</h2></div>
    <article class="media-featured-video">
      <div class="media-video-wrap">
        <iframe
          src="https://www.youtube.com/embed/AImN4DayCPo"
          title="MORIN Lab Featured Video"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen></iframe>
      </div>
      <div class="media-featured-meta">
        <p class="media-label">Featured Video</p>
        <h3 class="media-title">MBZIRC Maritime Grand Challenge (2024)</h3>
      </div>
    </article>
  </section>

  <section class="media-section">
    <div class="media-section-head">
      <h2>Videos</h2>
      <a class="media-view-all" href="{{ '/media/videos/' | relative_url }}">View all →</a>
    </div>
    <div class="media-grid">
      <article class="media-card">
        <a href="{{ '/media/videos/2024-MBZIRC-MGC/' | relative_url }}">
          <div class="media-thumb media-play"><img src="{{ '/assets/img/media/videos/2024-MBZIRC-MGC.jpeg' | relative_url }}" alt=""></div>
          <div class="media-card-meta"><p class="media-label">Video</p><h3 class="media-title">MBZIRC Maritime Grand Challenge (2024)</h3></div>
        </a>
      </article>
      <article class="media-card">
        <a href="{{ '/media/videos/2021-PohangExperiment/' | relative_url }}">
          <div class="media-thumb media-play"><img src="{{ '/assets/img/media/videos/2021-PohangExperiment.jpg' | relative_url }}" alt=""></div>
          <div class="media-card-meta"><p class="media-label">Video</p><h3 class="media-title">Field Experiments in Pohang Canal (2021)</h3></div>
        </a>
      </article>
      <article class="media-card">
        <a href="{{ '/media/videos/2019-VirtualRobotX/' | relative_url }}">
          <div class="media-thumb media-play"><img src="{{ '/assets/img/media/videos/2019-VirtualRobotX.jpg' | relative_url }}" alt=""></div>
          <div class="media-card-meta"><p class="media-label">Video</p><h3 class="media-title">Virtual RobotX Competition (2019)</h3></div>
        </a>
      </article>
    </div>
  </section>

  <section class="media-section">
    <div class="media-section-head">
      <h2>Gallery</h2>
      <a class="media-view-all" href="{{ '/media/gallery/' | relative_url }}">View all →</a>
    </div>
    <div class="media-grid">
      <article class="media-card">
        <a href="{{ '/media/gallery/2026-06-morin-kmrts/' | relative_url }}">
          <div class="media-thumb"><img src="{{ '/assets/img/media/gallery/gallery-01.jpg' | relative_url }}" alt="MORIN KMRTS"></div>
          <div class="media-card-meta"><p class="media-label">2026-06</p><h3 class="media-title">MORIN KMRTS</h3></div>
        </a>
      </article>
      <article class="media-card">
        <a href="{{ '/media/gallery/2025-05-morin-strawberry-party/' | relative_url }}">
          <div class="media-thumb"><img src="{{ '/assets/img/media/gallery/gallery-02.jpg' | relative_url }}" alt="MORIN Strawberry Party"></div>
          <div class="media-card-meta"><p class="media-label">2025-05</p><h3 class="media-title">MORIN Strawberry Party</h3></div>
        </a>
      </article>
      <article class="media-card">
        <a href="{{ '/media/gallery/2024-02-2024-kroc/' | relative_url }}">
          <div class="media-thumb"><img src="{{ '/assets/img/media/gallery/gallery-03.jpg' | relative_url }}" alt="2024 KRoC"></div>
          <div class="media-card-meta"><p class="media-label">2024-02</p><h3 class="media-title">2024 KRoC</h3></div>
        </a>
      </article>
    </div>
  </section>
</div>
