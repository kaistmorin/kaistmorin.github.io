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

/* Full hero, centered in viewport, with fixed max width */
.morin-hero-wrap {
  width: min(1600px, 100vw);
  margin-left: 50%;
  transform: translateX(-50%);
  position: relative;
  aspect-ratio: 2172 / 724;
  overflow: hidden;
  background: #eaf0f6;
}

/* Two image slides */
.morin-hero-slide {
  position: absolute;
  inset: 0;
  opacity: 0;
  transition: opacity 1.1s ease-in-out;
}

.morin-hero-slide.active {
  opacity: 1;
}

.morin-hero-slide img {
  width: 100%;
  height: 100%;
  object-fit: contain;   /* never crop */
  display: block;
}

/* Matching text overlays */
.morin-hero-content {
  position: absolute;
  left: clamp(34px, 6vw, 96px);
  top: 50%;
  transform: translateY(-50%);
  max-width: 650px;
  z-index: 5;
  opacity: 0;
  transition: opacity 1.1s ease-in-out;
  pointer-events: none;
}

.morin-hero-content.active {
  opacity: 1;
}

.morin-hero h1 {
  margin: 0;
  font-size: clamp(2.15rem, 4vw, 4.2rem);
  line-height: 1.06;
  font-weight: 700;
  letter-spacing: -0.03em;
}

.morin-hero-rule {
  width: 68px;
  height: 4px;
  margin: 22px 0 18px;
}

.morin-hero-tagline {
  margin: 0;
  font-size: clamp(1.05rem, 1.45vw, 1.42rem);
  line-height: 1.45;
}

/* Dark image -> white text */
.light-text h1,
.light-text .morin-hero-tagline {
  color: #fff;
  text-shadow: 0 2px 10px rgba(0,0,0,.30);
}

.light-text .morin-hero-rule {
  background: #1a8cff;
}

/* Light image -> dark text */
.dark-text h1,
.dark-text .morin-hero-tagline {
  color: #10233f;
  text-shadow: 0 1px 3px rgba(255,255,255,.30);
}

.dark-text .morin-hero-rule {
  background: #10233f;
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

/* KAIST above MORIN */
.morin-brand-stack {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 28px;
}

.morin-brand-stack .kaist-logo {
  width: min(250px, 88%);
  height: auto;
  display: block;
}

.morin-brand-stack .morin-logo {
  width: min(260px, 90%);
  height: auto;
  display: block;
}

@media (max-width: 900px) {
  .morin-hero-content {
    left: 24px;
    right: 24px;
    max-width: 70%;
  }

  .morin-hero h1 {
    font-size: clamp(1.55rem, 6vw, 2.6rem);
  }

  .morin-hero-tagline {
    font-size: .93rem;
  }

  .morin-intro-grid {
    grid-template-columns: 1fr;
    gap: 28px;
  }

  .morin-brand-stack {
    align-items: flex-start;
  }

  .morin-brand-stack .kaist-logo {
    width: 200px;
  }

  .morin-brand-stack .morin-logo {
    width: 210px;
  }
}
</style>

<div class="morin-home">

  <section class="morin-hero">
    <div class="morin-hero-wrap">

      <div class="morin-hero-slide active" id="morin-slide-dark">
        <img src="{{ '/assets/img/morin-hero-dark.png' | relative_url }}" alt="MORIN Lab marine robotics">
      </div>

      <div class="morin-hero-slide" id="morin-slide-light">
        <img src="{{ '/assets/img/morin-hero-light.png' | relative_url }}" alt="MORIN Lab civilian marine robotics">
      </div>

      <div class="morin-hero-content light-text active" id="morin-text-dark">
        <h1>Mobile Robotics &amp;<br>Intelligence Laboratory</h1>
        <div class="morin-hero-rule"></div>
        <p class="morin-hero-tagline">
          Intelligent autonomy for mobile systems<br>
          in complex and uncertain environments.
        </p>
      </div>

      <div class="morin-hero-content dark-text" id="morin-text-light">
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

      <div class="morin-brand-stack">
        <img class="kaist-logo"
             src="{{ '/assets/img/KAIST-logo.png' | relative_url }}"
             alt="KAIST">
        <img class="morin-logo"
             src="{{ '/assets/img/morin-logo.png' | relative_url }}"
             alt="MORIN Lab">
      </div>
    </div>
  </section>

</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const darkSlide = document.getElementById("morin-slide-dark");
  const lightSlide = document.getElementById("morin-slide-light");
  const darkText = document.getElementById("morin-text-dark");
  const lightText = document.getElementById("morin-text-light");

  let showingDark = true;

  setInterval(function () {
    showingDark = !showingDark;

    darkSlide.classList.toggle("active", showingDark);
    darkText.classList.toggle("active", showingDark);

    lightSlide.classList.toggle("active", !showingDark);
    lightText.classList.toggle("active", !showingDark);
  }, 5000);
});
</script>
