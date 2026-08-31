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
  padding: 44px 0 72px;
  font-family: inherit;
}
.contact-page h1,
.contact-page h2,
.contact-page h3,
.contact-page p { font-family: inherit; }
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
.contact-list { border-top: 1px solid var(--morin-line); }
.contact-item {
  display: grid;
  grid-template-columns: 170px minmax(0,1fr);
  gap: 24px;
  padding: 20px 0;
  border-bottom: 1px solid var(--morin-line);
}
.contact-label {
  color: var(--morin-muted);
  font-size: .9rem;
  line-height: 1.45;
}
.contact-title {
  margin: 0 0 7px;
  color: var(--morin-navy);
  font-size: 1.02rem;
  font-weight: 600;
  line-height: 1.4;
}
.contact-body {
  margin: 0;
  color: var(--morin-text);
  font-size: .9rem;
  line-height: 1.55;
}
@media (max-width: 640px) {
  .contact-page { width: calc(100% - 30px); }
  .contact-item { grid-template-columns: 1fr; gap: 5px; }
}
</style>

<div class="contact-page">
  <h1>Contact</h1>
  <p class="contact-intro">
    Contact information for the Mobile Robotics &amp; Intelligence Laboratory at KAIST.
  </p>

  <div class="contact-list">

    <article class="contact-item">
      <div class="contact-label">Laboratory</div>
      <div>
        <h2 class="contact-title">Mobile Robotics &amp; Intelligence Laboratory</h2>
        <p class="contact-body">Department of Mechanical Engineering, KAIST</p>
      </div>
    </article>

    <article class="contact-item">
      <div class="contact-label">Address</div>
      <div>
        <p class="contact-body">291 Daehak-ro, Yuseong-gu, Daejeon 305-701, Republic of Korea</p>
      </div>
    </article>

    <article class="contact-item">
      <div class="contact-label">Office</div>
      <div>
        <p class="contact-body">3105, Eureka Building (N27)</p>
        <p class="contact-body">4170, Practice Building (N9)</p>
      </div>
    </article>

    <article class="contact-item">
      <div class="contact-label">Student Office</div>
      <div>
        <p class="contact-body">4170, Practice Building (N9)</p>
      </div>
    </article>

    <article class="contact-item">
      <div class="contact-label">Phone</div>
      <div>
        <p class="contact-body">+82-42-350-1519</p>
      </div>
    </article>

    <article class="contact-item">
      <div class="contact-label">Fax</div>
      <div>
        <p class="contact-body">+82-42-350-1510</p>
      </div>
    </article>

    <article class="contact-item">
      <div class="contact-label">E-mail</div>
      <div>
        <p class="contact-body"><a href="mailto:jinwhan@kaist.ac.kr">jinwhan@kaist.ac.kr</a></p>
        <p class="contact-body" style="margin-top:6px;">The best and easiest way to reach me is by e-mail.</p>
      </div>
    </article>

  </div>
</div>
