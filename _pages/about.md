---
layout: default
title: MORIN Lab
permalink: /
nav: false
---

<style>
.morin-home {
  --morin-navy: #0b2d5c;
  --morin-blue: #1267d6;
  --morin-text: #14213d;
}

/* Escape al-folio's narrow content column and center the hero in the viewport */
.morin-hero-wrap {
  width: min(1600px, 100vw);
  margin-left: 50%;
  transform: translateX(-50%);
  position: relative;
  overflow: hidden;
}

/* Keep the full image visible: no cover-cropping */
.morin-hero-wrap img {
  width: 100%;
  height: auto;
  display: block;
}

/* Text overlay */
.morin-hero-content {
  position: absolute;
  left: clamp(36px, 6vw, 96px);
  top: 50%;
  transform: translateY(-50%);
  max-width: 680px;
  z-index: 2;
}

.morin-hero h1 {
  margin: 0;
  color: #fff;
  font-size: clamp(2.2rem, 4vw, 4.3rem);
  line-height: 1.06;
  font-weight: 700;
  letter-spacing: -0.03em;
  text-shadow: 0 2px 10px rgba(0,0,0,.30);
}

.morin-hero-rule {
  width: 68px;
  height: 4px;
  background: #1a8cff;
  margin: 22px 0 18px;
}

.morin-hero-tagline {
  margin: 0;
  color: #fff;
  font-size: clamp(1.05rem, 1.45vw, 1.42rem);
  line-height: 1.45;
  text-shadow: 0 2px 8px rgba(0,0,0,.28);
}

/* Intro */
.morin-intro {
  width: min(1080px, calc(100% - 48px));
  margin: 0 auto;
  padding: 42px 0 56px;
}

.morin-intro-grid {
  display: grid;
  grid-template-columns: minmax(0, 700px) minmax(220px, 280px);
  justify-content: center;
  gap: 56px;
  align-items: center;
}

.morin-intro-rule {
  width: 42px;
  height: 3px;
  background: var(--morin-blue);
  margin-bottom: 14px;
}

.morin-intro h2 {
  color: var(--morin-navy);
  font-size: 2rem;
  margin: 0 0 20px;
  font-weight: 700;
}

.morin-intro p {
  color: var(--morin-text);
  font-size: 1.05rem;
  line-height: 1.66;
  margin: 0 0 17px;
}

.morin-contact a {
  color: var(--morin-blue);
  text-decoration: none;
}

.morin-logo-wrap {
  display: flex;
  justify-content: center;
  align-items: center;
}

.morin-logo-wrap img {
  width: min(260px, 90%);
  height: auto;
  display: block;
}

@media (max-width: 900px) {
  .morin-hero-content {
    left: 24px;
    right: 24px;
    max-width: 68%;
  }

  .morin-hero h1 {
    font-size: clamp(1.65rem, 6vw, 2.8rem);
  }

  .morin-hero-tagline {
    font-size: .95rem;
  }

  .morin-intro-grid {
    grid-template-columns: 1fr;
    gap: 24px;
  }

  .morin-logo-wrap {
    justify-content: flex-start;
  }

  .morin-logo-wrap img {
    width: 220px;
  }
}
</style>

<div class="morin-home">

  <section class="morin-hero">
    <div class="morin-hero-wrap">
      <img src="{{ '/assets/img/morin-hero-dark.png' | relative_url }}" alt="MORIN Lab marine robotics">
      <div class="morin-hero-content">
        <h1>Mobile Robotics &amp;<br>Intelligence Laboratory</h1>
        <div class="morin-hero-rule"></div>
        <p class="morin-hero-tagline">
          Intelligent autonomy for mobile systems<br>
          in complex and uncertain environments.
        </p>
      </div>
    </div>
  </section>

  <section class="morin-intro">
    <div class="morin-intro-grid">
      <div>
        <div class="morin-intro-rule"></div>
        <h2>MORIN Lab at KAIST</h2>

        <p>
          Mobile Robotics &amp; Intelligence Laboratory (MORIN Lab) conducts research on
          intelligent control, autonomy, and decision-making for vehicles and mobile robotic systems.
        </p>

        <p>
          Our work spans dynamics, guidance, navigation, control, estimation, and learning-based
          methods, with a particular emphasis on marine robotic systems and autonomous vehicles.
        </p>

        <p>
          We develop fundamental algorithms and practical technologies that enable mobile robots
          to operate safely, robustly, and intelligently in complex and uncertain environments.
          While much of our research is motivated by marine applications—including autonomous
          surface and underwater vehicles—the methods we develop are broadly applicable to ground,
          aerial, and other mobile robotic systems.
        </p>

        <p class="morin-contact">
          For inquiries, please contact
          <a href="mailto:jinwhan@kaist.ac.kr">jinwhan@kaist.ac.kr</a>.
        </p>
      </div>

      <div class="morin-logo-wrap">
        <img src="{{ '/assets/img/morin-logo.png' | relative_url }}" alt="MORIN Lab">
      </div>
    </div>
  </section>

</div>
