---
layout: default
title: Videos
permalink: /media/videos/
nav: false
---

<style>
.media-archive{--morin-navy:#0b2d5c;--morin-text:#1f2937;--morin-muted:#667085;--morin-line:#e6ebf0;width:calc(100% - 48px);max-width:1120px;box-sizing:border-box;margin:0 auto;padding:11px 0 72px;font-family:inherit}
.media-archive h1{margin:0 0 12px;font-size:2.25rem;font-weight:400;line-height:1.15}
.media-intro{max-width:860px;margin:0 0 30px;color:var(--morin-text);font-size:1rem;line-height:1.55}
.archive-back{display:inline-block;margin:0 0 20px;color:var(--morin-navy);text-decoration:none;font-size:.9rem}.archive-back:hover{text-decoration:underline}
.archive-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:18px;margin-top:22px}
.archive-card{overflow:hidden;border:1px solid var(--morin-line);border-radius:8px;background:#fff}
.archive-card a{display:block;color:inherit;text-decoration:none}.archive-card a:hover .media-title{text-decoration:underline;text-underline-offset:2px}
.media-thumb{position:relative;overflow:hidden;aspect-ratio:16/9;background:#f3f5f7}.media-thumb img{display:block;width:100%;height:100%;object-fit:cover}
.media-play::after{content:"▶";position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);width:42px;height:42px;display:grid;place-items:center;padding-left:3px;border-radius:50%;background:rgba(11,45,92,.88);color:#fff;font-size:15px}
.archive-meta{padding:12px 13px 14px}.media-label{margin:0 0 5px;color:var(--morin-muted);font-size:.78rem}.media-title{margin:0;color:var(--morin-navy);font-size:1rem;font-weight:600;line-height:1.4}
@media(max-width:850px){.archive-grid{grid-template-columns:repeat(2,minmax(0,1fr))}}
@media(max-width:640px){.media-archive{width:calc(100% - 30px)}.archive-grid{grid-template-columns:1fr}}
</style>

<div class="media-archive">
  <a class="archive-back" href="{{ '/media/' | relative_url }}">← Back to Media</a>
  <h1>Videos</h1>
  <p class="media-intro">Selected videos from MORIN Lab research and activities</p>
  <div class="archive-grid">
    <article class="archive-card">
      <a href="{{ '/media/videos/2024-MBZIRC-MGC/' | relative_url }}">
        <div class="media-thumb media-play"><img src="{{ '/assets/img/media/videos/2024-MBZIRC-MGC.jpeg' | relative_url }}" alt=""></div>
        <div class="archive-meta"><p class="media-label">Video</p><h3 class="media-title">MBZIRC Maritime Grand Challenge (2024)</h3></div>
      </a>
    </article>
    <article class="archive-card">
      <a href="{{ '/media/videos/2021-PohangExperiment/' | relative_url }}">
        <div class="media-thumb media-play"><img src="{{ '/assets/img/media/videos/2021-PohangExperiment.jpg' | relative_url }}" alt=""></div>
        <div class="archive-meta"><p class="media-label">Video</p><h3 class="media-title">Field Experiments in Pohang Canal (2021)</h3></div>
      </a>
    </article>
    <article class="archive-card">
      <a href="{{ '/media/videos/2019-VirtualRobotX/' | relative_url }}">
        <div class="media-thumb media-play"><img src="{{ '/assets/img/media/videos/2019-VirtualRobotX.jpg' | relative_url }}" alt=""></div>
        <div class="archive-meta"><p class="media-label">Video</p><h3 class="media-title">Virtual RobotX Competition (2019)</h3></div>
      </a>
    </article>
    <article class="archive-card">
      <a href="{{ '/media/videos/2014-RobotXChallenge/' | relative_url }}">
        <div class="media-thumb media-play"><img src="{{ '/assets/img/media/videos/2014-RobotXChallenge.jpg' | relative_url }}" alt=""></div>
        <div class="archive-meta"><p class="media-label">Video</p><h3 class="media-title">Maritime RobotX Challenge (2014)</h3></div>
      </a>
    </article>
  </div>
</div>
