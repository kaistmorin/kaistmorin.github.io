---
layout: default
title: Media
permalink: /media/
nav: true
nav_order: 5
---

<style>
.media-page {
  --morin-navy: #0b2d5c;
  --morin-text: #1f2937;
  --morin-muted: #667085;
  --morin-line: #e6ebf0;
  width: calc(100% - 48px);
  max-width: 1120px;
  box-sizing: border-box;
  margin: 0 auto;
  padding: 11px 0 72px;
  font-family: inherit;
}

.media-page h1,
.media-page h2,
.media-page h3,
.media-page p,
.media-page button {
  font-family: inherit;
}

.media-page h1 {
  margin: 0 0 12px;
  color: inherit;
  font-size: 2.25rem;
  font-weight: 400;
  line-height: 1.15;
}

.media-intro {
  max-width: 820px;
  margin: 0 0 30px;
  color: var(--morin-text);
  font-size: 1rem;
  line-height: 1.55;
}

.media-section {
  margin-top: 34px;
}

.media-section-head {
  display: flex;
  align-items: center;
  gap: 14px;
  margin: 0 0 15px;
}

.media-section-head h2 {
  margin: 0;
  color: var(--morin-navy);
  font-size: 1.25rem;
  font-weight: 600;
  line-height: 1.3;
}

.media-section-head::after {
  content: "";
  flex: 1;
  height: 1px;
  background: var(--morin-line);
}

/* Featured: manually curated, not automatically selected */
.media-featured {
  display: grid;
  grid-template-columns: 1.55fr .95fr;
  gap: 18px;
}

.media-card {
  overflow: hidden;
  border: 1px solid var(--morin-line);
  border-radius: 9px;
  background: #fff;
}

.media-thumb {
  position: relative;
  overflow: hidden;
  aspect-ratio: 16 / 9;
  background: #f3f5f7;
}

.media-thumb img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.media-feature-main .media-thumb {
  aspect-ratio: 16 / 8.6;
}

.media-meta {
  padding: 13px 14px 15px;
}

.media-feature-main .media-meta {
  padding: 16px 17px 18px;
}

.media-label {
  margin: 0 0 5px;
  color: var(--morin-muted);
  font-size: .78rem;
  line-height: 1.35;
}

.media-title {
  margin: 0 0 6px;
  color: var(--morin-navy);
  font-size: 1rem;
  font-weight: 600;
  line-height: 1.4;
}

.media-feature-main .media-title {
  font-size: 1.08rem;
}

.media-desc {
  margin: 0;
  color: var(--morin-muted);
  font-size: .88rem;
  line-height: 1.5;
}

.media-side-stack {
  display: grid;
  gap: 18px;
}

.media-side-card {
  display: grid;
  grid-template-columns: 42% 58%;
}

.media-side-card .media-thumb {
  aspect-ratio: auto;
  min-height: 145px;
}

.media-side-card .media-meta {
  padding: 13px 14px;
}

.media-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 18px;
}

.media-link {
  display: block;
  color: inherit;
  text-decoration: none;
}

.media-link:hover .media-title {
  text-decoration: underline;
  text-underline-offset: 2px;
}

.media-play::after {
  content: "▶";
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  width: 46px;
  height: 46px;
  display: grid;
  place-items: center;
  padding-left: 3px;
  border-radius: 50%;
  background: rgba(11, 45, 92, .88);
  color: #fff;
  font-size: 16px;
  box-shadow: 0 2px 9px rgba(0,0,0,.16);
}

.media-gallery .media-card {
  border-radius: 8px;
}

.media-gallery .media-meta {
  padding: 11px 12px 13px;
}

.media-gallery .media-title {
  margin-bottom: 3px;
  font-size: .94rem;
}

@media (max-width: 850px) {
  .media-featured {
    grid-template-columns: 1fr;
  }

  .media-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}

@media (max-width: 640px) {
  .media-page {
    width: calc(100% - 30px);
  }

  .media-grid {
    grid-template-columns: 1fr;
  }

  .media-side-card {
    grid-template-columns: 40% 60%;
  }
}
</style>

<div class="media-page">
  <h1>Media</h1>
  <p class="media-intro">
    Selected highlights, activities, photos, and videos from MORIN Lab.
  </p>

  <!--
    FEATURED
    Manually curated. Keep only 2–3 representative items here.
    Replace image paths and links as better materials become available.
  -->
  <section class="media-section">
    <div class="media-section-head">
      <h2>Featured</h2>
    </div>

    <div class="media-featured">
      <article class="media-card media-feature-main">
        <a class="media-link" href="#" aria-label="Featured MORIN Lab research video">
          <div class="media-thumb media-play">
            <img src="{{ '/assets/img/media/featured-research.jpg' | relative_url }}"
                 alt="MORIN Lab research demonstration">
          </div>
          <div class="media-meta">
            <p class="media-label">Featured Video</p>
            <h3 class="media-title">MORIN Lab Research in Action</h3>
            <p class="media-desc">
              Selected field experiments and demonstrations in autonomous marine and mobile robotics.
            </p>
          </div>
        </a>
      </article>

      <div class="media-side-stack">
        <article class="media-card media-side-card">
          <div class="media-thumb">
            <img src="{{ '/assets/img/media/highlight-conference.jpg' | relative_url }}"
                 alt="MORIN Lab conference participation">
          </div>
          <div class="media-meta">
            <p class="media-label">Conference</p>
            <h3 class="media-title">Conference Highlights</h3>
            <p class="media-desc">Selected presentations and international activities.</p>
          </div>
        </article>

        <article class="media-card media-side-card">
          <div class="media-thumb">
            <img src="{{ '/assets/img/media/highlight-award.jpg' | relative_url }}"
                 alt="MORIN Lab award">
          </div>
          <div class="media-meta">
            <p class="media-label">Award</p>
            <h3 class="media-title">Awards &amp; Recognition</h3>
            <p class="media-desc">Selected awards and notable achievements.</p>
          </div>
        </article>
      </div>
    </div>
  </section>

  <!--
    HIGHLIGHTS
    Formal / outward-facing activities:
    awards, notable conference participation, invited talks, major demonstrations, etc.
  -->
  <section class="media-section">
    <div class="media-section-head">
      <h2>Highlights</h2>
    </div>

    <div class="media-grid">
      <article class="media-card">
        <div class="media-thumb">
          <img src="{{ '/assets/img/media/highlight-conference.jpg' | relative_url }}"
               alt="Conference activity">
        </div>
        <div class="media-meta">
          <p class="media-label">Conference</p>
          <h3 class="media-title">International Conference Activities</h3>
          <p class="media-desc">Presentations, sessions, and academic exchanges.</p>
        </div>
      </article>

      <article class="media-card">
        <div class="media-thumb">
          <img src="{{ '/assets/img/media/highlight-award.jpg' | relative_url }}"
               alt="Award activity">
        </div>
        <div class="media-meta">
          <p class="media-label">Award</p>
          <h3 class="media-title">Awards &amp; Recognition</h3>
          <p class="media-desc">Selected achievements by MORIN Lab members.</p>
        </div>
      </article>

      <article class="media-card">
        <div class="media-thumb">
          <img src="{{ '/assets/img/media/gallery-orchestra.jpg' | relative_url }}"
               alt="Special academic event">
        </div>
        <div class="media-meta">
          <p class="media-label">Special Event</p>
          <h3 class="media-title">Academic &amp; Community Events</h3>
          <p class="media-desc">Selected events involving the lab and research community.</p>
        </div>
      </article>
    </div>
  </section>

  <!--
    GALLERY
    Informal and visual archive:
    group photos, workshops, hiking, celebrations, lab events, and videos.
  -->
  <section class="media-section media-gallery">
    <div class="media-section-head">
      <h2>Gallery</h2>
    </div>

    <div class="media-grid">
      <article class="media-card">
        <div class="media-thumb">
          <img src="{{ '/assets/img/media/gallery-lab-event.jpg' | relative_url }}"
               alt="MORIN Lab group event">
        </div>
        <div class="media-meta">
          <p class="media-label">Lab Event</p>
          <h3 class="media-title">MORIN Lab Gathering</h3>
        </div>
      </article>

      <article class="media-card">
        <div class="media-thumb">
          <img src="{{ '/assets/img/media/gallery-outdoor.jpg' | relative_url }}"
               alt="MORIN Lab outdoor activity">
        </div>
        <div class="media-meta">
          <p class="media-label">Lab Life</p>
          <h3 class="media-title">Outdoor Activities</h3>
        </div>
      </article>

      <article class="media-card">
        <div class="media-thumb">
          <img src="{{ '/assets/img/media/gallery-kickoff.jpg' | relative_url }}"
               alt="MORIN Lab workshop">
        </div>
        <div class="media-meta">
          <p class="media-label">Workshop</p>
          <h3 class="media-title">Workshops &amp; Kickoffs</h3>
        </div>
      </article>

      <article class="media-card">
        <div class="media-thumb">
          <img src="{{ '/assets/img/media/gallery-hiking.jpg' | relative_url }}"
               alt="MORIN Lab hiking">
        </div>
        <div class="media-meta">
          <p class="media-label">Lab Life</p>
          <h3 class="media-title">Hiking &amp; Team Activities</h3>
        </div>
      </article>

      <article class="media-card">
        <a class="media-link" href="#" aria-label="MORIN Lab video">
          <div class="media-thumb media-play">
            <img src="{{ '/assets/img/media/featured-research.jpg' | relative_url }}"
                 alt="MORIN Lab video thumbnail">
          </div>
          <div class="media-meta">
            <p class="media-label">Video</p>
            <h3 class="media-title">Research &amp; Lab Videos</h3>
          </div>
        </a>
      </article>
    </div>
  </section>
</div>
