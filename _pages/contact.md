---
layout: default
title: Contact
permalink: /contact/
nav: true
nav_order: 6
---

<style>
.contact-page {
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

.contact-page h1,
.contact-page h2,
.contact-page p,
.contact-page a {
  font-family: inherit;
}

.contact-page h1 {
  margin: 0 0 12px;
  color: inherit;
  font-size: 2.25rem;
  font-weight: 400;
  line-height: 1.15;
}

.contact-intro {
  max-width: 900px;
  margin: 0 0 28px;
  color: var(--morin-text);
  font-size: 1rem;
  line-height: 1.55;
}

.contact-list {
  width: 100%;
  border-top: 1px solid var(--morin-line);
}

.contact-row {
  display: grid;
  grid-template-columns: 150px minmax(0, 1fr);
  gap: 24px;
  padding: 18px 0;
  border-bottom: 1px solid var(--morin-line);
}

.contact-label {
  color: var(--morin-muted);
  font-size: .9rem;
  line-height: 1.45;
}

.contact-value {
  margin: 0;
  color: var(--morin-text);
  font-size: .95rem;
  line-height: 1.55;
}

.contact-value strong {
  color: var(--morin-navy);
  font-weight: 600;
}

.contact-map-block {
  margin-top: 28px;
}

.contact-map-title {
  margin: 0 0 14px;
  color: var(--morin-navy);
  font-size: 1.35rem;
  font-weight: 600;
  line-height: 1.35;
}

.contact-map-link {
  display: block;
  line-height: 0;
}

.contact-map-image {
  display: block;
  width: 100%;
  height: auto;
  border: 1px solid var(--morin-line);
  border-radius: 12px;
}

@media (max-width: 640px) {
  .contact-page {
    width: calc(100% - 30px);
  }

  .contact-row {
    grid-template-columns: 1fr;
    gap: 5px;
  }
}
</style>

<div class="contact-page">
  <h1>Contact</h1>

  <p class="contact-intro">
    Contact information for the Mobile Robotics &amp; Intelligence Laboratory at KAIST.
  </p>

  <div class="contact-list">
    <div class="contact-row">
      <div class="contact-label">Laboratory</div>
      <p class="contact-value">
        <strong>Mobile Robotics &amp; Intelligence Laboratory</strong><br>
        Department of Mechanical Engineering, KAIST
      </p>
    </div>

    <div class="contact-row">
      <div class="contact-label">Address</div>
      <p class="contact-value">
        291 Daehak-ro, Yuseong-gu, Daejeon 34141, Republic of Korea
      </p>
    </div>

    <div class="contact-row">
      <div class="contact-label">Office</div>
      <p class="contact-value">
        4170, Practice Building (N9)
      </p>
    </div>

    <div class="contact-row">
      <div class="contact-label">Phone</div>
      <p class="contact-value">
        +82-42-350-1579
      </p>
    </div>
  </div>

  <div class="contact-map-block">
    <h2 class="contact-map-title">Location</h2>
    <a
      class="contact-map-link"
      href="https://www.google.com/maps/search/?api=1&query=KAIST+N9"
      target="_blank"
      rel="noopener"
      aria-label="Open KAIST N9 in Google Maps">
      <img
        class="contact-map-image"
        src="{{ '/assets/img/kaist-n9-map.png' | relative_url }}"
        alt="Map showing KAIST N9, Practice Building, on the KAIST main campus">
    </a>
  </div>
</div>
