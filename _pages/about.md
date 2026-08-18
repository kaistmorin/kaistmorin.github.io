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

/* Full-width hero. Text is already included in the hero image. */
.morin-hero {
  width: 100vw;
  margin-left: calc(50% - 50vw);
  height: clamp(300px, 31vw, 470px);
  background: url('{{ "/assets/img/morin-hero.png" | relative_url }}') center center / cover no-repeat;
}

/* Intro section */
.morin-intro {
  width: min(1180px, calc(100% - 48px));
  margin: 0 auto;
  padding: 48px 0 54px;
}

.morin-intro-grid {
  display: grid;
  grid-template-columns: minmax(0, 1.85fr) minmax(230px, .65fr);
  gap: 42px;
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

.morin-contact {
  margin-top: 24px !important;
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
  width: min(300px, 90%);
  height: auto;
  display: block;
}

@media (max-width: 900px) {
  .morin-hero {
    height: 320px;
    background-position: center center;
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

  <section class="morin-hero" aria-label="MORIN Lab marine robotics"></section>

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
