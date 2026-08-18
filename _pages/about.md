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
  --morin-frame: min(1180px, calc(100% - 64px));
}

/* Hero outer wrapper */
.morin-hero-outer {
  width: 100%;
  margin: 0;
  padding: 0;
}

/* Hero itself */
.morin-hero {
  width: var(--morin-frame);
  height: clamp(320px, 34vw, 520px);
  margin: 0 auto;
  position: relative;
  overflow: hidden;
  background:
    linear-gradient(90deg, rgba(6, 23, 52, 0.52) 0%, rgba(6, 23, 52, 0.28) 32%, rgba(6, 23, 52, 0.10) 55%, rgba(6, 23, 52, 0.06) 100%),
    url('{{ "/assets/img/morin-hero.png" | relative_url }}') center center / cover no-repeat;
}

/* Text overlay on hero */
.morin-hero-content {
  position: absolute;
  left: clamp(28px, 5vw, 80px);
  top: 50%;
  transform: translateY(-50%);
  max-width: 620px;
  z-index: 2;
}

.morin-hero h1 {
  margin: 0;
  color: #ffffff;
  font-size: clamp(2.2rem, 4.2vw, 4.4rem);
  line-height: 1.06;
  font-weight: 700;
  letter-spacing: -0.03em;
  text-shadow: 0 2px 10px rgba(0,0,0,0.28);
}

.morin-hero-rule {
  width: 68px;
  height: 4px;
  background: #1a8cff;
  margin: 22px 0 18px;
}

.morin-hero-tagline {
  margin: 0;
  color: rgba(255,255,255,0.96);
  font-size: clamp(1.1rem, 1.5vw, 1.45rem);
  line-height: 1.45;
  max-width: 520px;
  text-shadow: 0 2px 8px rgba(0,0,0,0.24);
}

/* Intro section */
.morin-intro {
  width: var(--morin-frame);
  margin: 0 auto;
  padding: 44px 0 54px;
}

.morin-intro-grid {
  display: grid;
  grid-template-columns: minmax(0, 700px) minmax(220px, 280px);
  justify-content: center;
  gap: 64px;
  align-items: center;
}

.morin-intro-text {
  max-width: 700px;
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
  width: min(260px, 90%);
  height: auto;
  display: block;
}

@media (max-width: 900px) {
  .morin-home {
    --morin-frame: calc(100% - 32px);
  }

  .morin-hero {
    height: 300px;
    background-position: center center;
  }

  .morin-hero-content {
    left: 24px;
    right: 24px;
    max-width: none;
  }

  .morin-intro-grid {
    grid-template-columns: 1fr;
    gap: 24px;
  }

  .morin-intro-text {
    max-width: none;
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

  <section class="morin-hero-outer">
    <div class="morin-hero">
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
      <div class="morin-intro-text">
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
