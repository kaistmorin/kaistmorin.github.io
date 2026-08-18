---
layout: page
title: Home
permalink: /
nav: false
---

<style>
/* MORIN home page */
.morin-home {
  --morin-navy: #0b2d5c;
  --morin-blue: #1267d6;
  --morin-text: #14213d;
}

/* Full-width hero */
.morin-hero {
  width: 100vw;
  margin-left: calc(50% - 50vw);
  min-height: 460px;
  background:
    linear-gradient(90deg, rgba(4, 28, 61, 0.78) 0%, rgba(4, 28, 61, 0.40) 45%, rgba(4, 28, 61, 0.06) 72%),
    url('{{ "/assets/img/morin-hero.png" | relative_url }}') center center / cover no-repeat;
  position: relative;
  display: flex;
  align-items: center;
}

.morin-hero-inner {
  width: min(1180px, calc(100% - 48px));
  margin: 0 auto;
  padding: 54px 0 64px;
}

.morin-hero h1 {
  margin: 0;
  color: #fff;
  font-size: clamp(2.4rem, 4.4vw, 4.5rem);
  line-height: 1.08;
  font-weight: 700;
  letter-spacing: -0.035em;
  max-width: 760px;
}

.morin-hero-rule {
  width: 70px;
  height: 4px;
  background: #1a8cff;
  margin: 24px 0 22px;
}

.morin-hero-tagline {
  margin: 0;
  color: rgba(255,255,255,.96);
  font-size: clamp(1.15rem, 1.65vw, 1.55rem);
  line-height: 1.45;
  max-width: 560px;
}

/* Introduction */
.morin-intro {
  max-width: 1180px;
  margin: 0 auto;
  padding: 52px 0 56px;
}

.morin-intro-grid {
  display: grid;
  grid-template-columns: minmax(0, 1.65fr) minmax(240px, .65fr);
  gap: 54px;
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
  margin: 0 0 22px;
  font-weight: 700;
}

.morin-intro p {
  color: var(--morin-text);
  font-size: 1.05rem;
  line-height: 1.65;
  margin: 0 0 18px;
}

.morin-contact {
  margin-top: 26px !important;
}

.morin-contact a {
  color: var(--morin-blue);
  text-decoration: none;
}

.morin-logo-wrap {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 170px;
}

.morin-logo-wrap img {
  width: min(320px, 88%);
  height: auto;
  display: block;
  filter: saturate(.92) contrast(1.03);
}

@media (max-width: 900px) {
  .morin-hero {
    min-height: 390px;
    background-position: 62% center;
  }

  .morin-intro-grid {
    grid-template-columns: 1fr;
    gap: 28px;
  }

  .morin-logo-wrap {
    justify-content: flex-start;
    min-height: 0;
  }

  .morin-logo-wrap img {
    width: 230px;
  }
}
</style>

<div class="morin-home">

  <section class="morin-hero">
    <div class="morin-hero-inner">
      <h1>Mobile Robotics &amp;<br>Intelligence Laboratory</h1>
      <div class="morin-hero-rule"></div>
      <p class="morin-hero-tagline">
        Intelligent autonomy for mobile systems<br>
        in complex and uncertain environments.
      </p>
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
