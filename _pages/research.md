---
layout: default
title: Research
permalink: /research/
nav: true
nav_order: 2
---

<style>
.research-page {
  --morin-navy: #0b2d5c;
  --morin-text: #1f2937;
  --morin-line: #e6ebf0;

  width: min(1120px, calc(100% - 48px));
  margin: 0 auto;
  padding: 38px 0 72px;
  font-family: inherit;
}

.research-page h1,
.research-page h2,
.research-page p,
.research-page li {
  font-family: inherit;
}

.research-page h1 {
  margin: 0 0 14px;
  color: inherit;
  font-size: 2.25rem;
  font-weight: 400;
  line-height: 1.15;
}

.research-intro {
  max-width: 900px;
  margin: 0 0 34px;
  color: var(--morin-text);
  font-size: 1rem;
  line-height: 1.55;
}

.research-list {
  border-top: 1px solid var(--morin-line);
}

.research-item {
  display: grid;
  grid-template-columns: 260px minmax(0, 1fr);
  gap: 34px;
  align-items: center;
  padding: 24px 0;
  border-bottom: 1px solid var(--morin-line);
}

.research-image {
  width: 100%;
  aspect-ratio: 16 / 9;
  overflow: hidden;
  background: #fff;
}

.research-image img {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
}

.research-item h2 {
  margin: 0 0 12px;
  color: var(--morin-navy);
  font-size: 1.25rem;
  font-weight: 600;
  line-height: 1.3;
}

.research-item ul {
  margin: 0;
  padding-left: 1.3rem;
}

.research-item li {
  margin: 7px 0;
  color: var(--morin-text);
  font-size: .98rem;
  line-height: 1.5;
}

@media (max-width: 760px) {
  .research-page {
    width: min(100% - 30px, 1120px);
  }

  .research-item {
    grid-template-columns: 1fr;
    gap: 18px;
  }

  .research-image {
    max-width: 440px;
  }
}
</style>

<div class="research-page">

  <h1>Research</h1>

  <p class="research-intro">
    MORIN Lab studies autonomy and intelligence for mobile robotic systems, with a strong emphasis on marine applications.
    Our research is organized around four closely related themes spanning dynamics and control, autonomous ship operations,
    navigation and mapping, and cooperative robotic systems.
  </p>

  <div class="research-list">

    <section class="research-item">
      <div class="research-image">
        <img src="{{ '/assets/img/research/marine-field-robotics.jpg' | relative_url }}" alt="Autonomous marine and field robotics">
      </div>
      <div>
        <h2>Autonomous Marine &amp; Field Robotics</h2>
        <ul>
          <li>Dynamics, guidance and control of USVs/UUVs</li>
          <li>Theoretical and learning-based modeling and control</li>
        </ul>
      </div>
    </section>

    <section class="research-item">
      <div class="research-image">
        <img src="{{ '/assets/img/research/mass.jpg' | relative_url }}" alt="Maritime autonomous surface ships">
      </div>
      <div>
        <h2>Maritime Autonomous Surface Ships (MASS)</h2>
        <ul>
          <li>Maritime situational awareness and automated ship operations</li>
          <li>COLREGs-compliant collision avoidance, reachability-based safety analysis</li>
        </ul>
      </div>
    </section>

    <section class="research-item">
      <div class="research-image">
        <img src="{{ '/assets/img/research/slam.jpg' | relative_url }}" alt="Navigation, mapping and SLAM">
      </div>
      <div>
        <h2>Navigation, Mapping &amp; SLAM in Challenging Environments</h2>
        <ul>
          <li>Navigation and mapping in GPS-denied environments</li>
          <li>Geophysical navigation &amp; SLAM in underwater environment</li>
        </ul>
      </div>
    </section>

    <section class="research-item">
      <div class="research-image">
        <img src="{{ '/assets/img/research/multi-robot.jpg' | relative_url }}" alt="Multi-robot coordination and mission planning">
      </div>
      <div>
        <h2>Multi-Robot Coordination &amp; Mission Planning</h2>
        <ul>
          <li>Multi-vehicle planning, task allocation and scheduling</li>
          <li>Informative path planning for search and mapping missions</li>
        </ul>
      </div>
    </section>

  </div>

</div>
