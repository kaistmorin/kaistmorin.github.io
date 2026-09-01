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
  padding: 22px 0 72px;
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
  margin: 0 0 36px;
  color: var(--morin-text);
  font-size: 1rem;
  line-height: 1.55;
}

.contact-list {
  width: 100%;
  border-top: 1px solid #e6ebf0;
}

.contact-row {
  display: grid;
  grid-template-columns: 150px minmax(0, 1fr);
  gap: 24px;
  padding: 18px 0;
  border-bottom: 1px solid #e6ebf0;
}

.contact-label {
  color: #667085;
  font-size: .9rem;
  line-height: 1.45;
}

.contact-value {
  margin: 0;
  color: #1f2937;
  font-size: .95rem;
  line-height: 1.55;
}

.contact-value strong {
  color: #0b2d5c;
  font-weight: 600;
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
      <p class="contact-value"><strong>Mobile Robotics &amp; Intelligence Laboratory</strong><br>Department of Mechanical Engineering, KAIST</p>
    </div>

    <div class="contact-row">
      <div class="contact-label">Address</div>
      <p class="contact-value">291 Daehak-ro, Yuseong-gu, Daejeon 305-701, Republic of Korea</p>
    </div>

    <div class="contact-row">
      <div class="contact-label">Office</div>
      <p class="contact-value">3105, Eureka Building (N27)<br>4170, Practice Building (N9)</p>
    </div>

    <div class="contact-row">
      <div class="contact-label">Student office</div>
      <p class="contact-value">4170, Practice Building (N9)</p>
    </div>

    <div class="contact-row">
      <div class="contact-label">Phone</div>
      <p class="contact-value">+82-42-350-1519</p>
    </div>

    <div class="contact-row">
      <div class="contact-label">Fax</div>
      <p class="contact-value">+82-42-350-1510</p>
    </div>

    <div class="contact-row">
      <div class="contact-label">E-mail</div>
      <p class="contact-value"><a href="mailto:jinwhan@kaist.ac.kr">jinwhan@kaist.ac.kr</a><br>The best and easiest way to reach me is by e-mail.</p>
    </div>
  </div>
</div>
