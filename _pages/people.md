---
layout: default
title: People
permalink: /people/
nav: true
nav_order: 3
---

<style>
.people-page {
  --morin-navy: #0b2d5c;
  --morin-blue: #1267d6;
  --morin-text: #17233a;
  --morin-muted: #667085;
  --morin-line: #e8edf2;
  width: min(1180px, calc(100% - 48px));
  margin: 0 auto;
  padding: 34px 0 70px;
}

.people-page h1 {
  margin: 0 0 6px;
  color: var(--morin-navy);
  font-size: 2.35rem;
  font-weight: 700;
}

.people-lead {
  margin: 0 0 42px;
  color: var(--morin-muted);
  font-size: 1.02rem;
}

.people-section {
  margin-top: 44px;
}

.people-section:first-of-type {
  margin-top: 0;
}

.people-section-title {
  display: flex;
  align-items: center;
  gap: 14px;
  margin: 0 0 18px;
}

.people-section-title h2 {
  margin: 0;
  color: var(--morin-navy);
  font-size: 1.35rem;
  font-weight: 700;
}

.people-section-title::after {
  content: "";
  height: 1px;
  flex: 1;
  background: var(--morin-line);
}

.people-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 20px;
}

.person-card {
  border: 1px solid var(--morin-line);
  border-radius: 14px;
  background: #fff;
  overflow: hidden;
  box-shadow: 0 4px 14px rgba(12, 39, 75, 0.035);
}

.person-photo {
  aspect-ratio: 1 / 1;
  background: #f5f7f9;
  overflow: hidden;
}

.person-photo img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.person-info {
  padding: 17px 17px 18px;
}

.person-name {
  margin: 0;
  color: var(--morin-navy);
  font-size: 1.02rem;
  font-weight: 700;
}

.person-role {
  margin: 3px 0 12px;
  color: var(--morin-blue);
  font-size: .87rem;
  font-weight: 600;
}

.person-meta {
  margin: 0 0 6px;
  color: var(--morin-text);
  font-size: .84rem;
  line-height: 1.48;
}

.person-meta strong {
  font-weight: 600;
}

.person-email {
  display: inline-block;
  margin-top: 8px;
  color: var(--morin-muted);
  font-size: .80rem;
  text-decoration: none;
  overflow-wrap: anywhere;
}

.person-email:hover {
  color: var(--morin-blue);
}

.faculty-grid {
  grid-template-columns: minmax(0, 560px);
}

.faculty-card {
  display: grid;
  grid-template-columns: 170px 1fr;
}

.faculty-card .person-photo {
  aspect-ratio: auto;
  min-height: 210px;
}

.faculty-card .person-info {
  padding: 24px;
}

.faculty-card .person-name {
  font-size: 1.22rem;
}

.admin-grid {
  grid-template-columns: repeat(3, minmax(0, 1fr));
}

@media (max-width: 1000px) {
  .people-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }
}

@media (max-width: 760px) {
  .people-page {
    width: min(100% - 30px, 1180px);
  }

  .people-grid,
  .admin-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .faculty-grid {
    grid-template-columns: 1fr;
  }

  .faculty-card {
    grid-template-columns: 130px 1fr;
  }
}

@media (max-width: 520px) {
  .people-grid,
  .admin-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="people-page">

  <h1>People</h1>
  <p class="people-lead">Members of the Mobile Robotics &amp; Intelligence Laboratory at KAIST.</p>

  <section class="people-section">
    <div class="people-section-title"><h2>Faculty</h2></div>
    <div class="people-grid faculty-grid">
      <article class="person-card faculty-card">
        <div class="person-photo">
          <img src="{{ '/assets/img/people/jinwhan-kim.jpg' | relative_url }}" alt="Jinwhan Kim">
        </div>
        <div class="person-info">
          <h3 class="person-name">Jinwhan Kim</h3>
          <div class="person-role">Professor</div>
          <p class="person-meta">Department of Mechanical Engineering, KAIST</p>
          <p class="person-meta"><strong>Research:</strong> Autonomous systems, guidance, navigation, control, estimation, and marine robotics</p>
          <a class="person-email" href="mailto:jinwhan@kaist.ac.kr">jinwhan@kaist.ac.kr</a>
        </div>
      </article>
    </div>
  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>Postdoctoral Researchers</h2></div>
    <div class="people-grid">
      <!-- Kyungseo Kim -->
      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/kyungseo-kim.jpg' | relative_url }}" alt="Kyungseo Kim"></div>
        <div class="person-info">
          <h3 class="person-name">Kyungseo Kim</h3>
          <div class="person-role">Postdoctoral Researcher</div>
          <p class="person-meta"><strong>Ph.D.:</strong> —</p>
          <a class="person-email" href="mailto:chalseokim@kaist.ac.kr">chalseokim@kaist.ac.kr</a>
        </div>
      </article>

      <!-- Jinwook Park -->
      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jinwook-park.jpg' | relative_url }}" alt="Jinwook Park"></div>
        <div class="person-info">
          <h3 class="person-name">Jinwook Park</h3>
          <div class="person-role">Postdoctoral Researcher</div>
          <p class="person-meta"><strong>Ph.D.:</strong> —</p>
          <a class="person-email" href="mailto:qkrwlsdnr10@kaist.ac.kr">qkrwlsdnr10@kaist.ac.kr</a>
        </div>
      </article>
    </div>
  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>Ph.D. Students</h2></div>
    <div class="people-grid">

      <!-- For Ph.D. students: fill B.S. and M.S. school/year when available. -->

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/sol-han.jpg' | relative_url }}" alt="Sol Han"></div>
        <div class="person-info">
          <h3 class="person-name">Sol Han</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <p class="person-meta"><strong>Research:</strong> Computer Vision · Sensor Fusion</p>
          <a class="person-email" href="mailto:dream4future@kaist.ac.kr">dream4future@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/qianyi-zhang.jpg' | relative_url }}" alt="Qianyi Zhang"></div>
        <div class="person-info">
          <h3 class="person-name">Qianyi Zhang</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:qianyizhang@kaist.ac.kr">qianyizhang@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/kiyong-park.jpg' | relative_url }}" alt="Kiyong Park"></div>
        <div class="person-info">
          <h3 class="person-name">Kiyong Park</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:qkrrldyd777@kaist.ac.kr">qkrrldyd777@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/donghyun-kim.jpg' | relative_url }}" alt="Donghyun Kim"></div>
        <div class="person-info">
          <h3 class="person-name">Donghyun Kim</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:rlaehdgusqwe@kaist.ac.kr">rlaehdgusqwe@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/hakmo-son.jpg' | relative_url }}" alt="Hakmo Son"></div>
        <div class="person-info">
          <h3 class="person-name">Hakmo Son</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:gkrah12@kaist.ac.kr">gkrah12@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jisu-jeon.jpg' | relative_url }}" alt="Jisu Jeon"></div>
        <div class="person-info">
          <h3 class="person-name">Jisu Jeon</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:dun04047@kaist.ac.kr">dun04047@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/dongwook-lee.jpg' | relative_url }}" alt="Dongwook Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Dongwook Lee</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <p class="person-meta"><strong>Research:</strong> Deep Learning · UUV SLAM</p>
          <a class="person-email" href="mailto:dongwooklee1201@kaist.ac.kr">dongwooklee1201@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jiyong-choi.jpg' | relative_url }}" alt="Jiyong Choi"></div>
        <div class="person-info">
          <h3 class="person-name">Jiyong Choi</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:jiyongchoi0702@kaist.ac.kr">jiyongchoi0702@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Minju Kang"></div>
        <div class="person-info">
          <h3 class="person-name">Minju Kang</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:mkang@kaist.ac.kr">mkang@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Keunhwan Kim"></div>
        <div class="person-info">
          <h3 class="person-name">Keunhwan Kim</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:khgapa@kaist.ac.kr">khgapa@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/yeongha-shin.jpg' | relative_url }}" alt="Yeongha Shin"></div>
        <div class="person-info">
          <h3 class="person-name">Yeongha Shin</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:yeongha.shin@kaist.ac.kr">yeongha.shin@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Wonseok Oh"></div>
        <div class="person-info">
          <h3 class="person-name">Wonseok Oh</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:ooww0123@kaist.ac.kr">ooww0123@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/kyeongmo-kang.jpg' | relative_url }}" alt="Kyeongmo Kang"></div>
        <div class="person-info">
          <h3 class="person-name">Kyeongmo Kang</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:kmkang@kaist.ac.kr">kmkang@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/ju-hang-lee.jpg' | relative_url }}" alt="Ju Hang Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Ju Hang Lee</h3>
          <div class="person-role">Ph.D. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>M.S.:</strong> —</p>
          <a class="person-email" href="mailto:hangsul@kaist.ac.kr">hangsul@kaist.ac.kr</a>
        </div>
      </article>

    </div>
  </section>

  <!--
  If any current student is actually in the Integrated M.S./Ph.D. program,
  move the corresponding card here and keep only the undergraduate degree:
  B.S.: University (Year)
  -->
  <section class="people-section">
    <div class="people-section-title"><h2>Integrated M.S./Ph.D. Students</h2></div>
    <div class="people-grid">
      <!-- Placeholder: move/add integrated-program students here. -->
    </div>
  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>M.S. Students</h2></div>
    <div class="people-grid">

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/taewoo-lee.jpg' | relative_url }}" alt="TaeWoo Lee"></div>
        <div class="person-info">
          <h3 class="person-name">TaeWoo Lee</h3>
          <div class="person-role">M.S. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <p class="person-meta"><strong>Research:</strong> Model Predictive Control</p>
          <a class="person-email" href="mailto:aimer1@kaist.ac.kr">aimer1@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/kyeonghun-lee.jpg' | relative_url }}" alt="Kyeonghun Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Kyeonghun Lee</h3>
          <div class="person-role">M.S. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <a class="person-email" href="mailto:rapael6696@kaist.ac.kr">rapael6696@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/sangwon-park.jpg' | relative_url }}" alt="SangWon Park"></div>
        <div class="person-info">
          <h3 class="person-name">SangWon Park</h3>
          <div class="person-role">M.S. Student</div>
          <p class="person-meta"><strong>B.S.:</strong> —</p>
          <a class="person-email" href="mailto:sangwon0730@kaist.ac.kr">sangwon0730@kaist.ac.kr</a>
        </div>
      </article>

    </div>
  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>Administration</h2></div>
    <div class="people-grid admin-grid">
      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/seonah-lee.jpg' | relative_url }}" alt="Seonah Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Seonah Lee</h3>
          <div class="person-role">Administrator</div>
          <p class="person-meta">Room 4170, Practice Building (N9)</p>
          <a class="person-email" href="mailto:gusdl814@kaist.ac.kr">gusdl814@kaist.ac.kr</a>
        </div>
      </article>
    </div>
  </section>

</div>
