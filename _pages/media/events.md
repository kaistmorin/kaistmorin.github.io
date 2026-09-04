---
layout: default
title: Events
permalink: /media/events/
nav: false
---

<style>
.media-page,.media-archive,.media-detail{
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
.media-page h1,.media-archive h1,.media-detail h1{
  margin:0 0 12px;font-size:2.25rem;font-weight:400;line-height:1.15;
}
.media-intro{max-width:860px;margin:0 0 30px;color:var(--morin-text);font-size:1rem;line-height:1.55}
.media-section{margin-top:34px}
.media-section-head{display:flex;align-items:center;gap:14px;margin:0 0 15px}
.media-section-head h2{margin:0;color:var(--morin-navy);font-size:1.25rem;font-weight:600}
.media-section-head::after{content:"";flex:1;height:1px;background:var(--morin-line)}
.media-view-all{margin-left:auto;color:var(--morin-navy);font-size:.86rem;font-weight:600;text-decoration:none;white-space:nowrap}
.media-view-all:hover,.archive-back:hover{text-decoration:underline}
.media-featured-video,.media-card,.archive-card{
  overflow:hidden;border:1px solid var(--morin-line);border-radius:8px;background:#fff;
}
.media-video-wrap{position:relative;width:100%;aspect-ratio:16/9;background:#000}
.media-video-wrap iframe{position:absolute;inset:0;width:100%;height:100%;border:0}
.media-featured-meta,.media-card-meta,.archive-meta{padding:12px 13px 14px}
.media-label,.detail-date{margin:0 0 5px;color:var(--morin-muted);font-size:.78rem}
.media-title{margin:0 0 5px;color:var(--morin-navy);font-size:1rem;font-weight:600;line-height:1.4}
.media-desc{margin:0;color:var(--morin-muted);font-size:.88rem;line-height:1.5}
.media-grid,.archive-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:18px}
.media-card a,.archive-card a{display:block;color:inherit;text-decoration:none}
.media-card a:hover .media-title,.archive-card a:hover .media-title{text-decoration:underline;text-underline-offset:2px}
.media-thumb{position:relative;overflow:hidden;aspect-ratio:16/9;background:#f3f5f7}
.media-thumb img{display:block;width:100%;height:100%;object-fit:cover}
.media-play::after{content:"▶";position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);width:42px;height:42px;display:grid;place-items:center;padding-left:3px;border-radius:50%;background:rgba(11,45,92,.88);color:#fff;font-size:15px}
.archive-back{display:inline-block;margin:0 0 20px;color:var(--morin-navy);text-decoration:none;font-size:.9rem}
.archive-grid{margin-top:22px}
.detail-hero{overflow:hidden;border:1px solid var(--morin-line);border-radius:8px;margin:18px 0 24px}
.detail-hero img{display:block;width:100%;max-height:620px;object-fit:cover}
.detail-body{max-width:860px;color:var(--morin-text);font-size:.98rem;line-height:1.7}
.detail-body p{margin:0 0 14px}
.detail-actions{margin-top:18px}
.detail-actions a{color:var(--morin-navy);font-weight:600;text-decoration:none}
.detail-actions a:hover{text-decoration:underline}
@media(max-width:850px){.media-grid,.archive-grid{grid-template-columns:repeat(2,minmax(0,1fr))}}
@media(max-width:640px){.media-page,.media-archive,.media-detail{width:calc(100% - 30px)}.media-grid,.archive-grid{grid-template-columns:1fr}}
</style>

<div class="media-archive">
  <a class="archive-back" href="{{ '/media/' | relative_url }}">← Back to Media</a>
  <h1>Events</h1>
  <p class="media-intro">Awards, conference activities, workshops, competitions, and other notable MORIN Lab events.</p>
  <div class="archive-grid">
  <article class="archive-card">
    <a href="{{ '/media/events/2026-07-15-dongwook-lee-best-application-paper-award-candidate-at-ur-2026/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-01.jpg' | relative_url }}" alt="Dongwook Lee — Best Application Paper Award Candidate at UR 2026"></div>
      <div class="archive-meta">
        <p class="media-label">2026-07-15</p>
        <h3 class="media-title">Dongwook Lee — Best Application Paper Award Candidate at UR 2026</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2026-07-02-taekjoong-kwon-best-paper-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-02.jpg' | relative_url }}" alt="Taekjoong Kwon — Best Paper Award"></div>
      <div class="archive-meta">
        <p class="media-label">2026-07-02</p>
        <h3 class="media-title">Taekjoong Kwon — Best Paper Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2025-09-29-taewoo-lee-student-excellent-poster-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-03.jpg' | relative_url }}" alt="Taewoo Lee — Student Excellent Poster Award"></div>
      <div class="archive-meta">
        <p class="media-label">2025-09-29</p>
        <h3 class="media-title">Taewoo Lee — Student Excellent Poster Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2025-06-18-dongwook-lee-third-prize-at-oceans-25-student-poster-competition/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-04.jpg' | relative_url }}" alt="Dongwook Lee — Third Prize at OCEANS&#x27;25 Student Poster Competition"></div>
      <div class="archive-meta">
        <p class="media-label">2025-06-18</p>
        <h3 class="media-title">Dongwook Lee — Third Prize at OCEANS'25 Student Poster Competition</h3>
      </div>
    </a>
  </article></div>
</div>
