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
  /* Fix width against the viewport, not the theme's parent container. */
  width: min(1120px, calc(100vw - 48px));
  max-width: none;
  box-sizing: border-box;
  margin-left: 50%;
  margin-right: 0;
  transform: translateX(-50%);
  padding: 44px 0 72px;
  font-family: inherit;
}
.contact-page h1,
.contact-page h2,
.contact-page p,
.contact-page a { font-family: inherit; }
.contact-page h1 {
  margin: 0 0 12px;
  color: inherit;
  font-size: 2.25rem;
  font-weight: 400;
  line-height: 1.15;
}
.contact-intro {
  max-width: 900px;
  margin: 0 0 36px;
  color: var(--morin-text);
  font-size: 1rem;
  line-height: 1.55;
}
.contact-grid {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(320px, 0.9fr);
  gap: 32px;
  width: 100%;
  border-top: 1px solid var(--morin-line);
  padding-top: 24px;
}
.contact-block h2 {
  margin: 0 0 12px;
  color: var(--morin-navy);
  font-size: 1.22rem;
  font-weight: 600;
  line-height: 1.35;
}
.contact-block p {
  margin: 0 0 8px;
  color: var(--morin-text);
  font-size: .95rem;
  line-height: 1.55;
}
.contact-label {
  display: inline-block;
  min-width: 105px;
  color: var(--morin-muted);
}
.contact-note {
  margin-top: 18px !important;
  color: var(--morin-muted) !important;
  font-size: .9rem !important;
}
@media (max-width: 720px) {
  .contact-page { width: calc(100vw - 30px); }
  .contact-grid { grid-template-columns: 1fr; gap: 28px; }
}

.contact-block {
  min-width: 0;
}

</style>

<div class="contact-page">
  <h1>Contact</h1>
  <p class="contact-intro">Contact information for the Mobile Robotics &amp; Intelligence Laboratory at KAIST.</p>

  <div class="contact-grid">
    <section class="contact-block">
      <h2>Mobile Robotics &amp; Intelligence Laboratory</h2>
      <p>Department of Mechanical Engineering, KAIST</p>
      <p>291 Daehak-ro, Yuseong-gu, Daejeon 305-701, Republic of Korea</p>

      <p style="margin-top:20px;"><span class="contact-label">Office</span>3105, Eureka Building (N27)</p>
      <p><span class="contact-label">Office</span>4170, Practice Building (N9)</p>
      <p><span class="contact-label">Student office</span>4170, Practice Building (N9)</p>
    </section>

    <section class="contact-block">
      <h2>Contact</h2>
      <p><span class="contact-label">Phone</span>+82-42-350-1519</p>
      <p><span class="contact-label">Fax</span>+82-42-350-1510</p>
      <p><span class="contact-label">E-mail</span><a href="mailto:jinwhan@kaist.ac.kr">jinwhan@kaist.ac.kr</a></p>
      <p class="contact-note">The best and easiest way to reach me is by e-mail.</p>
    </section>
  </div>
</div>
