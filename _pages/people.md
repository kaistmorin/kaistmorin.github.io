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
  --morin-text: #1f2937;
  --morin-muted: #667085;
  --morin-line: #e6ebf0;
  --morin-sky: #1f8fd0;
  width: calc(100% - 48px);
  max-width: 1120px;
  box-sizing: border-box;
  margin: 0 auto;
  padding: 11px 0 72px;
  font-family: inherit;
}

.people-page h1,
.people-page h2,
.people-page h3,
.people-page p,
.people-page a,
.people-page td,
.people-page th {
  font-family: inherit;
}

.people-page h1 {
  margin: 0 0 12px;
  color: inherit;
  font-size: 2.25rem;
  font-weight: 400;
  line-height: 1.15;
}

.people-intro {
  max-width: 900px;
  margin: 0 0 36px;
  color: var(--morin-text);
  font-size: 1rem;
  line-height: 1.55;
}

.people-section {
  margin-top: 42px;
}

.people-section-title {
  display: flex;
  align-items: center;
  gap: 14px;
  margin-bottom: 18px;
}

.people-section-title h2 {
  margin: 0;
  color: var(--morin-navy);
  font-size: 1.35rem;
  font-weight: 600;
}

.people-section-title::after {
  content: "";
  height: 1px;
  flex: 1;
  background: var(--morin-line);
}

.people-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 24px;
}

.person-card {
  display: flex;
  flex-direction: column;
  height: 100%;
  border: 1px solid var(--morin-line);
  border-radius: 12px;
  background: #fff;
  overflow: hidden;
}

.person-photo {
  width: 100%;
  aspect-ratio: 1 / 1;
  background: #fff;
  overflow: hidden;
}

.person-photo img {
  width: 100%;
  height: 100%;
  object-fit: contain;
  object-position: center;
  display: block;
  background: #fff;
}

.person-info {
  display: flex;
  flex: 1;
  flex-direction: column;
  padding: 17px 17px 19px;
}

.person-name {
  margin: 0 0 8px;
  color: var(--morin-navy);
  font-size: 1.02rem;
  font-weight: 600;
}

.person-role {
  display: inline-block;
  margin: -3px 0 10px;
  padding: 3px 8px;
  border-radius: 5px;
  background: #f3f4f6;
  color: var(--morin-blue);
  font-size: .88rem;
}

.person-affiliation {
  margin: 0 0 8px;
  color: #4b5563;
  font-size: .88rem;
  line-height: 1.4;
}

.person-affiliation a {
  color: var(--morin-blue);
  font-weight: 600;
  text-decoration: none;
}

.person-affiliation a:hover {
  color: var(--morin-sky);
  text-decoration: underline;
}

.person-name-affiliation {
  margin-left: 6px;
  color: #4b5563;
  font-size: .88rem;
  font-weight: 400;
}

.person-name-affiliation a {
  color: var(--morin-blue);
  font-weight: 600;
  text-decoration: none;
}

.person-name-affiliation a:hover {
  color: var(--morin-sky);
  text-decoration: underline;
}

.person-meta,
.person-email {
  margin: 0 0 5px;
  color: var(--morin-text);
  font-size: .86rem;
  line-height: 1.5;
}

.person-email:hover {
  color: var(--morin-muted);
}

.person-email {
  display: inline-block;
  margin-top: 7px;
  color: var(--morin-muted);
  text-decoration: none;
  overflow-wrap: anywhere;
}

.person-homepage {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 22px;
  height: 22px;
  margin-left: 7px;
  border: 1px solid #c7d9f5;
  border-radius: 999px;
  background: #eaf1fd;
  color: var(--morin-blue);
  font-size: .68rem;
  line-height: 1;
  text-decoration: none;
  vertical-align: middle;
  transition: background-color .15s ease, border-color .15s ease, color .15s ease;
}

.person-homepage:hover,
.person-homepage:focus-visible {
  border-color: var(--morin-blue);
  background: var(--morin-blue);
  color: #fff;
  text-decoration: none;
}

.person-interests {
  display: flex;
  flex-wrap: wrap;
  gap: 5px;
  margin: 9px 0 0;
}

.person-interest {
  padding: 3px 9px;
  border-radius: 5px;
  background: #f3f4f6;
  color: #4b5563;
  font-size: .78rem;
  line-height: 1.45;
  white-space: nowrap;
}

.person-info-spacer {
  flex: 1;
  min-height: 12px;
}

.person-latest {
  width: 100%;
  margin: 0;
  padding: 11px 0 0;
  border-top: 1px dashed var(--morin-line);
}

.person-latest > summary {
  display: flex;
  align-items: center;
  gap: 6px;
  margin: 0;
  color: var(--morin-blue);
  cursor: pointer;
  font-size: .71rem;
  font-weight: 700;
  letter-spacing: .05em;
  line-height: 1.4;
  list-style: none;
  text-transform: uppercase;
}

/* Hide the native disclosure triangle; the caret below replaces it. */
.person-latest > summary::-webkit-details-marker {
  display: none;
}

.person-latest > summary:hover,
.person-latest > summary:focus-visible {
  color: var(--morin-navy);
}

.person-latest .person-latest-caret {
  font-size: .6rem;
  transition: transform .18s ease;
}

.person-latest[open] .person-latest-caret {
  transform: rotate(180deg);
}

.person-latest .person-latest-body {
  margin: 7px 0 0;
}

.person-latest .person-latest-more {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  margin-top: 7px;
  color: var(--morin-blue);
  font-size: .78rem;
  font-weight: 600;
  text-decoration: none;
}

.person-latest .person-latest-more:hover,
.person-latest .person-latest-more:focus-visible {
  color: var(--morin-sky);
  text-decoration: underline;
}

.person-latest .person-latest-title {
  margin: 0 0 3px;
  color: var(--morin-navy);
  font-size: .84rem;
  font-weight: 600;
  line-height: 1.42;
}

.person-latest .person-latest-venue {
  margin: 0;
  color: var(--morin-muted);
  font-size: .8rem;
  font-style: italic;
  line-height: 1.42;
}

.director-card {
  display: grid;
  grid-template-columns: 220px minmax(0, 1fr);
  gap: 28px;
  align-items: start;
  border: 1px solid var(--morin-line);
  border-radius: 12px;
  padding: 22px;
  background: #fff;
}

.director-photo {
  width: 220px;
  aspect-ratio: 1 / 1;
  object-fit: contain;
  background: #fff;
}

.director-card h3 {
  margin: 0 0 5px;
  color: var(--morin-navy);
  font-size: 1.25rem;
  font-weight: 600;
}

.director-card h4 {
  margin: 18px 0 6px;
  color: var(--morin-navy);
  font-size: .95rem;
  font-weight: 600;
}

.director-card p {
  margin: 0 0 4px;
  color: var(--morin-text);
  font-size: .88rem;
  line-height: 1.5;
}

.alumni-wrap {
  overflow-x: auto;
  border-top: 1px solid var(--morin-line);
}

.alumni-table {
  width: 100%;
  border-collapse: collapse;
  font-size: .88rem;
}

.alumni-table th,
.alumni-table td {
  padding: 9px 10px;
  border-bottom: 1px solid var(--morin-line);
  text-align: left;
  vertical-align: top;
}

.alumni-table th {
  color: var(--morin-navy);
  font-weight: 600;
  background: #fafbfc;
}

@media (max-width: 900px) {
  .people-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
}

@media (max-width: 680px) {
  .people-page { width: calc(100% - 30px); }
  .people-grid { grid-template-columns: 1fr; }
  .director-card { grid-template-columns: 1fr; }
  .director-photo { width: 180px; }
}
</style>

<div class="people-page">

  <h1>People</h1>
  <p class="people-intro">
    Members of the Mobile Robotics &amp; Intelligence Laboratory at KAIST.
  </p>

  <section class="people-section">
    <div class="people-section-title"><h2>Director &amp; Professor</h2></div>

    <div class="director-card">
      <img class="director-photo" src="{{ '/assets/img/people/jinwhan-kim.jpg' | relative_url }}" alt="Jinwhan Kim">
      <div>
        <h3>Jinwhan Kim</h3>
        <p><strong>Professor</strong>, Department of Mechanical Engineering, KAIST</p>
        <p>Jointly affilated with Robotics Program & Graduate School of Ocean Systems Engineering</p>
        <p><strong>Phone</strong>: +82-42-350-1519</p>
        <p><strong>Email</strong>: jinwhan@kaist.ac.kr</p>

        <h4>Education</h4>
        <p><strong>Ph.D.</strong> Aeronautics and Astronautics (w/ Ph.D. Minor in Electrical Eng.), Stanford University</p>
        <p><strong>M.S.</strong> Naval Architecture and Ocean Engineering, Seoul National University</p>
        <p><strong>B.S.</strong> Naval Architecture and Ocean Engineering, Seoul National University</p>
      </div>
    </div>

  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>Postdoctoral Researchers</h2></div>
    <div class="people-grid">

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/kyungseokim.png' | relative_url }}" alt="Kyungseo Kim"></div>
        <div class="person-info">
          <h3 class="person-name">Kyungseo Kim</h3>
          <p class="person-meta"><strong>Ph.D.</strong> KAIST (2026)</p>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">chalseokim@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jinwookpark.png' | relative_url }}" alt="Jinwook Park"></div>
        <div class="person-info">
          <h3 class="person-name">Jinwook Park</h3>
          <p class="person-meta"><strong>Ph.D.</strong> KAIST</p>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">qkrwlsdnr10@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/qianyizhang.png' | relative_url }}" alt="Qianyi Zhang"></div>
        <div class="person-info">
          <h3 class="person-name">Qianyi Zhang</h3>
          <p class="person-meta"><strong>Ph.D.</strong> KAIST</p>
          <p class="person-meta"><strong>M.S.</strong> Harbin Engineering University</p>
          <p class="person-meta"><strong>B.S.</strong> Harbin Engineering University</p>
          <a class="person-email">qianyizhang@kaist.ac.kr</a>
        </div>
      </article>

    </div>

  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>Ph.D. Students</h2></div>
    <div class="people-grid">

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/solhan.png' | relative_url }}" alt="Sol Han"></div>
        <div class="person-info">
        <h3 class="person-name">Sol Han <a class="person-homepage" href="https://solhan.notion.site/" target="_blank" rel="noopener" aria-label="Homepage" title="Homepage"><i class="fa-solid fa-arrow-up-right-from-square"></i></a></h3>
        <p class="person-meta"><strong>B.S.</strong> KAIST</p>
        <div class="person-interests">
          <span class="person-interest">Computer Vision</span>
          <span class="person-interest">Sensor Fusion</span>
        </div>
        <a class="person-email" >dream4future@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/kiyongpark.png' | relative_url }}" alt="Kiyong Park"></div>
        <div class="person-info">
        <h3 class="person-name">Kiyong Park</h3>
        <p class="person-meta"><strong>B.S.</strong> KAIST</p>
        <a class="person-email">qkrrldyd777@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/donghyunkim.png' | relative_url }}" alt="Donghyun Kim"></div>
        <div class="person-info">
        <h3 class="person-name">Donghyun Kim</h3>
        <p class="person-meta"><strong>M.S.</strong> KAIST</p>
        <p class="person-meta"><strong>B.S.</strong> KAIST</p>
        <a class="person-email">rlaehdgusqwe@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/hakmoson.png' | relative_url }}" alt="Hakmo Son"></div>
        <div class="person-info">
        <h3 class="person-name">Hakmo Son</h3>
        <p class="person-meta"><strong>B.S.</strong> KAIST</p>
        <a class="person-email">gkrah12@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jisujeon.png' | relative_url }}" alt="Jisu Jeon"></div>
        <div class="person-info">
        <h3 class="person-name">Jisu Jeon</h3>
        <p class="person-meta"><strong>M.S.</strong> Korea University</p>
        <p class="person-meta"><strong>B.S.</strong> Korea University</p>
        <a class="person-email">dun04047@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/dongwooklee.jpg' | relative_url }}" alt="Dongwook Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Dongwook Lee</h3>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> Jacobs University Bremen</p>
          <div class="person-interests">
            <span class="person-interest">Deep Learning</span>
            <span class="person-interest">UUV SLAM</span>
          </div>
          <a class="person-email">dongwooklee1201@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jiyongchoi.png' | relative_url }}" alt="Jiyong Choi"></div>
        <div class="person-info">
          <h3 class="person-name">Jiyong Choi</h3>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">jiyongchoi0702@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/Minju.jpg' | relative_url }}" alt="Minju Kang"></div>
        <div class="person-info">
          <h3 class="person-name">Minju Kang
          <span class="person-name-affiliation">
          (w/
          <a href="https://www.kriso.re.kr/" target="_blank" rel="noopener">KRISO</a>
          )
          </span>
          </h3>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">mkang@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/Keunhwan.jpg' | relative_url }}" alt="Keunhwan Kim"></div>
        <div class="person-info">
          <h3 class="person-name">Keunhwan Kim
          <span class="person-name-affiliation">
          (w/
          <a href="https://www.keti.re.kr/" target="_blank" rel="noopener">KETI</a>
          )
          </span>
          </h3>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> Hanyang University</p>
          <a class="person-email">khgapa@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/yeonghashin.png' | relative_url }}" alt="Yeongha Shin"></div>
        <div class="person-info">
          <h3 class="person-name">Yeongha Shin <a class="person-homepage" href="https://www.linkedin.com/in/yeongha-shin-672665234/" target="_blank" rel="noopener" aria-label="Homepage" title="Homepage"><i class="fa-solid fa-arrow-up-right-from-square"></i></a></h3>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> <span title="Korea Maritime and Ocean University">KMOU</span></p>
          <div class="person-interests">
            <span class="person-interest" title="Scene Understanding">Scene Underst.</span>
            <span class="person-interest">Decision Making</span>
          </div>
          <a class="person-email">yeongha.shin@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/Wonseok.png' | relative_url }}" alt="Wonseok Oh"></div>
        <div class="person-info">
          <h3 class="person-name">Wonseok Oh
          <span class="person-name-affiliation">
          (w/
          <a href="https://twinny.ai/" target="_blank" rel="noopener">Twinny</a>
          )
          </span>
          </h3>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <div class="person-interests">
            <span class="person-interest">SLAM</span>
            <span class="person-interest">VLA</span>
          </div>
          <a class="person-email">ooww0123@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/kyeongmokang.png' | relative_url }}" alt="Kyeongmo Kang"></div>
        <div class="person-info">
          <h3 class="person-name">Kyeongmo Kang
          <span class="person-name-affiliation">
          (w/
          <a href="https://www.navy.mil.kr/" target="_blank" rel="noopener">ROK Navy</a>
          )
          </span>
          </h3>
          <p class="person-meta"><strong>M.S.</strong> Texas A&M University</p>
          <p class="person-meta"><strong>B.S.</strong> ROK Naval Academy</p>
          <a class="person-email">kmkang@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/juhanglee.jpg' | relative_url }}" alt="Ju Hang Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Ju Hang Lee</h3>
          <p class="person-meta"><strong>B.S.</strong> Hanyang University</p>
          <a class="person-email">hangsul@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jisookim.jpg' | relative_url }}" alt="Ji Soo Kim"></div>
        <div class="person-info">
          <h3 class="person-name">Ji Soo Kim <a class="person-homepage" href="https://www.linkedin.com/in/ji-soo-kim-17824b161/" target="_blank" rel="noopener" aria-label="Homepage" title="Homepage"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
          <span class="person-name-affiliation">
            (w/
            <a href="https://www.hd-ksoe.com/" target="_blank" rel="noopener">HD KSOE</a>
            )
          </span>
        </h3>
        <!--
          <h3 class="person-name">Ji Soo Kim</h3>
          <p class="person-affiliation">Currently with <a href="https://www.hd-ksoe.com/" target="_blank" rel="noopener">HD KSOE</a></p>
        -->
          <p class="person-meta"><strong>M.S.</strong> Inha University</p>
          <p class="person-meta"><strong>B.S.</strong> Inha University</p>
          <div class="person-interests">
            <span class="person-interest">Software-defined Vessel</span>
          </div>
          <a class="person-email">kimjjs100@kaist.ac.kr</a>
        </div>
      </article>


    </div>

  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>M.S. Students</h2></div>
    <div class="people-grid">

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/taewoolee.jpg' | relative_url }}" alt="Tae Woo Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Tae Woo Lee</h3>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <div class="person-interests">
            <span class="person-interest">Model Predictive Control</span>
          </div>
          <a class="person-email">aimer1@kaist.ac.kr</a>
        </div>
      </article>

       <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/kyeonghunlee.png' | relative_url }}" alt="Kyeonghun Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Kyeonghun Lee</h3>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">rapael6696@kaist.ac.kr</a>
        </div>
      </article>

       <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/sangwonpark.png' | relative_url }}" alt="Sang Won Park"></div>
        <div class="person-info">
          <h3 class="person-name">Sang Won Park</h3>
          <p class="person-meta"><strong>B.S.</strong> Hanyang University</p>
          <a class="person-email">sangwon0730@kaist.ac.kr</a>
        </div>
      </article>

       <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/taeung.jpg' | relative_url }}" alt="Taeung Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Taeung Lee <a class="person-homepage" href="https://foodbanana.github.io/" target="_blank" rel="noopener" aria-label="Homepage" title="Homepage"><i class="fa-solid fa-arrow-up-right-from-square"></i></a></h3>
          <p class="person-meta"><strong>B.S.</strong> Korea University</p>
          <a class="person-email">christy201@kaist.ac.kr</a>
        </div>
      </article>

    </div>

  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>Administrator</h2></div>
    <div class="people-grid">
      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/seonahlee.png' | relative_url }}" alt="Seonah Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Seonah Lee</h3>
          <p class="person-meta"><strong>Office</strong>: 4170, Practice Building (N9)</p>
          <p class="person-meta"><strong>Phone</strong>: +82-42-350-1579</p>
          <a class="person-email">gusdl814@kaist.ac.kr</a>
        </div>
      </article>
    </div>
  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>Alumni</h2></div>
    <div class="alumni-wrap">
      <table class="alumni-table">
        <thead>
          <tr><th>Name</th><th>Year / Degree</th><th>Affiliation / Destination</th></tr>
        </thead>
        <tbody>
          <tr><td>Hyunkuen Cho</td><td>2026, Ph.D.</td><td>Avikus Co.</td></tr>
          <tr><td>Junwoo Park</td><td>2026, Master</td><td>Twinny</td></tr>
          <tr><td>Yonghoe Lee</td><td>2026, Master</td><td>Samsung Electronics</td></tr>
          <tr><td>Taekjoong Kwon</td><td>2026, Master</td><td>Republic of Korea Navy</td></tr>
          <tr><td>Haggi Do</td><td>2025, Ph.D.</td><td>Korea Institute of Machinery &amp; Materials</td></tr>
          <tr><td>Changyu Lee</td><td>2025, Ph.D.</td><td>Kongju National University</td></tr>
          <tr><td>Hoon Chung</td><td>2025, Master</td><td>MOBINN</td></tr>
          <tr><td>Junhyung Kim</td><td>2025, Master</td><td>LG Electronics Inc.</td></tr>
          <tr><td>Kunchul Hwang</td><td>2025, Ph.D.</td><td>Agency for Defense Development</td></tr>
          <tr><td>Dongha Chung</td><td>2024, Ph.D.</td><td>URobotics</td></tr>
          <tr><td>Youngbum Kim</td><td>2024, Ph.D.</td><td>HD Hyundai XiteSolution</td></tr>
          <tr><td>Jonghwi Kim</td><td>2024, Ph.D.</td><td>Korea Aerospace University</td></tr>
          <tr><td>Eunghyun Kim</td><td>2024, Master</td><td>Samsung Electronics</td></tr>
          <tr><td>Uijong Kim</td><td>2023, Master</td><td>Agency for Defense Development</td></tr>
          <tr><td>Jungwoo Han</td><td>2023, Master</td><td>Honda Research Institute</td></tr>
          <tr><td>Junwoo Jang</td><td>2023, Ph.D.</td><td>Inha University</td></tr>
          <tr><td>Jinsik Kim</td><td>2022, Master</td><td>GINT Co.</td></tr>
          <tr><td>Wonseok Oh</td><td>2022, Master</td><td>Twinny</td></tr>
          <tr><td>Yonghoon Cho</td><td>2021, Ph.D.</td><td>Agency for Defense Development</td></tr>
          <tr><td>Jisung Park</td><td>2021, Ph.D.</td><td>Gyeongsang National University</td></tr>
          <tr><td>Seungjo Hong</td><td>2021, Master</td><td>Republic of Korea Navy</td></tr>
          <tr><td>David Munk Zino</td><td>2020, Master</td><td>MAN Energy Solutions</td></tr>
          <tr><td>Jeonghyeon Wang</td><td>2020, Ph.D.</td><td>Samsung Electronics</td></tr>
          <tr><td>Keunhwan Kim</td><td>2020, Master</td><td>Korea Electronics Technology Institute</td></tr>
          <tr><td>Sukmin Yoon</td><td>2020, Ph.D.</td><td>Agency for Defense Development</td></tr>
          <tr><td>Seonghun Hong</td><td>2019, Ph.D.</td><td>Keimyung University</td></tr>
          <tr><td>Jungwook Han</td><td>2019, Ph.D.</td><td>Korea Research Institute of Ships and Ocean Engineering</td></tr>
          <tr><td>Byunghyun Yoo</td><td>2019, Ph.D.</td><td>Electronics and Telecommunications Research Institute</td></tr>
          <tr><td>Taeyun Kim</td><td>2019, Ph.D.</td><td>Agency for Defense Development</td></tr>
          <tr><td>Thorsteinn Baldvin Jonsson</td><td>2018, Master</td><td>Seoul Robotics</td></tr>
          <tr><td>Youngshik Kim</td><td>2018, Ph.D.</td><td>Korea Research Institute of Ships and Ocean Engineering</td></tr>
          <tr><td>Sangwook Woo</td><td>2017, Master</td><td>Hyundai Construction Equipment</td></tr>
          <tr><td>Aleixo Cambeiro Barreiro</td><td>2017, Master</td><td>Fraunhofer Heinrich-Hertz-Institute</td></tr>
          <tr><td>Soohyun Nam</td><td>2017, Ph.D.</td><td>Samsung Electronics</td></tr>
          <tr><td>Jaeheon Choe</td><td>2017, Ph.D.</td><td>Incheon National University</td></tr>
          <tr><td>Yeonjoo Shim</td><td>2016, Master</td><td>Hyundai Mobis</td></tr>
          <tr><td>Donghwan Kim</td><td>2016, Master</td><td>Moais</td></tr>
          <tr><td>Minju Kang</td><td>2016, Master</td><td>Korea Research Institute of Ships and Ocean Engineering</td></tr>
          <tr><td>Jeonghong Park</td><td>2016, Ph.D.</td><td>Korea Research Institute of Ships and Ocean Engineering</td></tr>
          <tr><td>Sungchur Kwon</td><td>2015, Master</td><td>EDGE Group</td></tr>
          <tr><td>Hojang Lee</td><td>2014, Master</td><td>Defence Agency for Technology and Quality</td></tr>
          <tr><td>Hyungbae Lee</td><td>2013, Master</td><td>Hyundai Heavy Industries</td></tr>
          <tr><td>Younghyun Kim</td><td>2012, Master</td><td>LIG D&A</td></tr>
          <tr><td>Quoc Van Tran</td><td>Postdoctoral Researcher</td><td>Hanoi University of Science and Technology</td></tr>
          <tr><td>Mohan Santhakumar</td><td>Postdoctoral Researcher</td><td>Indian Institute of Technology Palakkad</td></tr>
          <tr><td>Armagan Elibol</td><td>Postdoctoral Researcher</td><td>Forschungzentrum Jülich</td></tr>
        </tbody>
      </table>
    </div>
  </section>

</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  // Latest publication per member, resolved at page load so that adding a paper
  // to _data/publications.yml is the only edit needed.
  //   publications        - every paper, grouped by category
  //   publication_authors - member name spellings (English / Korean / aliases)
  //   highlight_venues    - "top venue" keywords, shared with the home page
  const publicationData = {{ site.data.publications | jsonify }};
  const authorRoster = {{ site.data.publication_authors | jsonify }};
  const topVenueKeywords = {{ site.data.highlight_venues.match | jsonify }};

  // Preference order, best first. Within "International Journals" a venue that
  // matches topVenueKeywords (RA-L, Transactions, ...) outranks the rest, so the
  // full order is: top journal > other international journal > international
  // conference > domestic journal > domestic conference. Ties go to the newest
  // year, then to the order the papers are written in _data/publications.yml
  // (newest first).
  const CATEGORY_ORDER = [
    "International Journals",
    "International Conferences",
    "Domestic Journals",
    "Domestic Conferences"
  ];

  function escapeHtml(value) {
    return String(value)
      .replace(/&/g, "&amp;")
      .replace(/</g, "&lt;")
      .replace(/>/g, "&gt;")
      .replace(/"/g, "&quot;")
      .replace(/'/g, "&#039;");
  }

  // Ignore case, spaces, hyphens and periods when matching a spelling.
  function normalizeName(value) {
    return String(value || "").replace(/[\s\-.]/g, "").toLowerCase();
  }

  // spelling -> canonical member name.
  const authorLookup = new Map();
  authorRoster.forEach(function (person) {
    [person.name].concat(person.korean || [], person.aliases || []).forEach(function (spelling) {
      authorLookup.set(normalizeName(spelling), person.name);
    });
  });

  // "Hakmo Son, Haggi Do and Jinwhan Kim*" -> canonical member names only.
  function memberAuthors(value) {
    const found = [];
    String(value || "")
      .split(/\s*,\s*|\s+and\s+/)
      .forEach(function (raw) {
        const canonical = authorLookup.get(normalizeName(raw.replace(/\*+$/, "")));
        if (canonical && found.indexOf(canonical) === -1) found.push(canonical);
      });
    return found;
  }

  function rankOf(category, venue) {
    const base = CATEGORY_ORDER.indexOf(category);
    if (base === -1) return CATEGORY_ORDER.length + 1;
    const top = category === "International Journals" && topVenueKeywords.some(function (keyword) {
      return String(venue || "").indexOf(keyword) !== -1;
    });
    return top ? 0 : base + 1;
  }

  function isBetter(candidate, current) {
    if (candidate.rank !== current.rank) return candidate.rank < current.rank;
    if (Number(candidate.year) !== Number(current.year)) return Number(candidate.year) > Number(current.year);
    return candidate.order < current.order;
  }

  // canonical member name -> the one paper to show on their card.
  const bestByMember = new Map();
  let order = 0;
  CATEGORY_ORDER.forEach(function (category) {
    (publicationData[category] || []).forEach(function (item) {
      const entry = {
        title: item.title,
        venue: item.venue,
        year: item.year,
        rank: rankOf(category, item.venue),
        order: order++
      };
      memberAuthors(item.authors).forEach(function (name) {
        const current = bestByMember.get(name);
        if (!current || isBetter(entry, current)) bestByMember.set(name, entry);
      });
    });
  });

  // Venue strings already end with the year; only add one when the venue has none.
  function venueLine(entry) {
    const venue = String(entry.venue || "").trim();
    if (!entry.year || /\b(19|20)\d{2}\b/.test(venue)) return venue;
    return venue.replace(/\.$/, "") + ", " + entry.year + ".";
  }

  // The heading also carries the homepage button and the affiliation note, so
  // only its own text nodes are the name. `data-person` overrides it.
  function cardName(card) {
    const explicit = card.getAttribute("data-person");
    if (explicit) return explicit;
    const heading = card.querySelector(".person-name") || card.querySelector("h3");
    if (!heading) return "";
    return Array.prototype.filter
      .call(heading.childNodes, function (node) { return node.nodeType === 3; })
      .map(function (node) { return node.textContent; })
      .join(" ")
      .replace(/\s+/g, " ")
      .trim();
  }

  // Deep link into the Publications page with this member preselected in its
  // author filter (see the query-param handling in _pages/publications.md).
  const publicationsUrl = "{{ '/publications/' | relative_url }}";

  // Member cards only: the director's own card deliberately has no latest paper.
  document.querySelectorAll(".person-card").forEach(function (card) {
    const member = authorLookup.get(normalizeName(cardName(card)));
    const entry = bestByMember.get(member);
    if (!entry) return;

    const target = card.querySelector(".person-info");
    if (!target) return;

    // <details> keeps the card compact: the paper shows only once the row is clicked.
    // The spacer eats the slack of an equal-height card so the row sits at the
    // bottom while keeping its gap above the dashed rule.
    target.insertAdjacentHTML("beforeend", `
          <div class="person-info-spacer"></div>
          <details class="person-latest">
            <summary>
              <span>Latest publication</span>
              <i class="fa-solid fa-chevron-down person-latest-caret" aria-hidden="true"></i>
            </summary>
            <div class="person-latest-body">
              <p class="person-latest-title">${escapeHtml(entry.title)}</p>
              <p class="person-latest-venue">${escapeHtml(venueLine(entry))}</p>
              <a class="person-latest-more" href="${publicationsUrl}?author=${encodeURIComponent(member)}">
                More publications
                <i class="fa-solid fa-arrow-right" aria-hidden="true"></i>
              </a>
            </div>
          </details>`);
  });

  // Every member card gets the same height, across sections too: CSS alone only
  // equalises cards that share a grid row. Cards with an expanded "Latest
  // publication" are skipped while measuring so opening one never ratchets the
  // shared height up.
  const cards = Array.from(document.querySelectorAll(".person-card"));

  function equalizeCardHeights() {
    cards.forEach(function (card) { card.style.minHeight = ""; });
    let tallest = 0;
    cards.forEach(function (card) {
      if (card.querySelector(".person-latest[open]")) return;
      tallest = Math.max(tallest, card.getBoundingClientRect().height);
    });
    if (!tallest) return;
    cards.forEach(function (card) { card.style.minHeight = tallest + "px"; });
  }

  equalizeCardHeights();

  // Re-measure on width changes; the details toggles are laid out inside the
  // already-fixed height, so they don't need to trigger one.
  let resizeTimer;
  let lastWidth = window.innerWidth;
  window.addEventListener("resize", function () {
    if (window.innerWidth === lastWidth) return;
    lastWidth = window.innerWidth;
    clearTimeout(resizeTimer);
    resizeTimer = setTimeout(equalizeCardHeights, 150);
  });

  // Webfonts land after this runs and can change text wrapping.
  if (document.fonts && document.fonts.ready) {
    document.fonts.ready.then(equalizeCardHeights);
  }
});
</script>
