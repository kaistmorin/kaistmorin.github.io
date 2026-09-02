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
  font-size: 0.9rem;
  line-height: 1.4;
}

.person-meta,
.person-email {
  margin: 0 0 5px;
  color: var(--morin-text);
  font-size: .86rem;
  line-height: 1.5;
}

.person-email {
  display: inline-block;
  margin-top: 7px;
  color: var(--morin-muted);
  text-decoration: none;
  overflow-wrap: anywhere;
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
        <div class="person-photo"><img src="{{ '/assets/img/people/kyungseo-kim.jpg' | relative_url }}" alt="Kyungseo Kim"></div>
        <div class="person-info">
          <h3 class="person-name">Kyungseo Kim</h3>
          <p class="person-meta"><strong>Ph.D.</strong> KAIST (2026)</p>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">chalseokim@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jinwook-park.jpg' | relative_url }}" alt="Jinwook Park"></div>
        <div class="person-info">
          <h3 class="person-name">Jinwook Park</h3>
          <p class="person-meta"><strong>Ph.D.</strong> KAIST</p>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">qkrwlsdnr10@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/qianyi-zhang.jpg' | relative_url }}" alt="Qianyi Zhang"></div>
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
        <div class="person-photo"><img src="{{ '/assets/img/people/sol-han.jpg' | relative_url }}" alt="Sol Han"></div>
        <div class="person-info">
        <h3 class="person-name">Sol Han</h3>
        <p class="person-meta"><strong>B.S.</strong> KAIST</p>
        <a class="person-email" >dream4future@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/kiyong-park.jpg' | relative_url }}" alt="Kiyong Park"></div>
        <div class="person-info">
        <h3 class="person-name">Kiyong Park</h3>
        <p class="person-meta"><strong>B.S.</strong> KAIST</p>
        <a class="person-email">qkrrldyd777@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/donghyun-kim.jpg' | relative_url }}" alt="Donghyun Kim"></div>
        <div class="person-info">
        <h3 class="person-name">Donghyun Kim</h3>
        <p class="person-meta"><strong>M.S.</strong> KAIST</p>
        <p class="person-meta"><strong>B.S.</strong> KAIST</p>
        <a class="person-email">rlaehdgusqwe@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/hakmo-son.jpg' | relative_url }}" alt="Hakmo Son"></div>
        <div class="person-info">
        <h3 class="person-name">Hakmo Son</h3>
        <p class="person-meta"><strong>B.S.</strong> KAIST</p>
        <a class="person-email">gkrah12@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jisu-jeon.jpg' | relative_url }}" alt="Jisu Jeon"></div>
        <div class="person-info">
        <h3 class="person-name">Jisu Jeon</h3>
        <p class="person-meta"><strong>M.S.</strong> Korea University</p>
        <p class="person-meta"><strong>B.S.</strong> Korea University</p>
        <a class="person-email">dun04047@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/dongwook-lee.jpg' | relative_url }}" alt="Dongwook Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Dongwook Lee</h3>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> Jacobs University Bremen</p>
          <a class="person-email">dongwooklee1201@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/jiyong-choi.jpg' | relative_url }}" alt="Jiyong Choi"></div>
        <div class="person-info">
          <h3 class="person-name">Jiyong Choi</h3>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">jiyongchoi0702@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Minju Kang"></div>
        <div class="person-info">
          <h3 class="person-name">Minju Kang</h3>
          <p class="person-affiliation">KRISO</p>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">mkang@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Keunhwan Kim"></div>
        <div class="person-info">
          <h3 class="person-name">Keunhwan Kim</h3>
          <p class="person-affiliation">KETI</p>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> Hanyang University</p>
          <a class="person-email">mkang@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Yeongha Shin"></div>
        <div class="person-info">
          <h3 class="person-name">Yeongha Shin</h3>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> Korea Maritime University</p>
          <a class="person-email">yeongha.shin@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Wonseok Oh"></div>
        <div class="person-info">
          <h3 class="person-name">Wonseok Oh</h3>
          <p class="person-affiliation">Tweeny</p>
          <p class="person-meta"><strong>M.S.</strong> KAIST</p>
          <p class="person-meta"><strong>B.S.</strong> KAIST</p>
          <a class="person-email">ooww0123@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Kyeongmo Kang"></div>
        <div class="person-info">
          <h3 class="person-name">Kyeongmo Kang</h3>
          <p class="person-affiliation">ROK Navy</p>
          <p class="person-meta"><strong>M.S.</strong> Texas A&M University</p>
          <p class="person-meta"><strong>B.S.</strong> ROK Naval Academy</p>
          <a class="person-email">kmkang@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Ju Hang Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Ju Hang Lee</h3>          
          <p class="person-meta"><strong>B.S.</strong> Hanyang University</p>
          <a class="person-email">hangsul@kaist.ac.kr</a>
        </div>
      </article>

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Ji Soo Kim"></div>
        <div class="person-info">
          <h3 class="person-name">Ji Soo Kim</h3>
          <p class="person-affiliation">HD KSOE</p>
          <p class="person-meta"><strong>M.S.</strong> Inha University</p>
          <p class="person-meta"><strong>B.S.</strong> Inha University</p>
          <a class="person-email">kimjjs100@kaist.ac.kr</a>
        </div>
      </article>

    </div>
  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>M.S. Students</h2></div>
    <div class="people-grid">

      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Tae Woo Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Tae Woo Lee</h3>
          <p class="person-meta">B.S.: KAIST (0000)</p>
          <a class="person-email">aimer1@kaist.ac.kr</a>
        </div>
      </article>

       <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Kyeonghun Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Kyeonghun Lee</h3>
          <p class="person-meta">B.S.: KAIST (0000)</p>
          <a class="person-email">rapael6696@kaist.ac.kr</a>
        </div>
      </article>

       <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Sang Won Park"></div>
        <div class="person-info">
          <h3 class="person-name">Sang Won Park</h3>
          <p class="person-meta">B.S.: Hanyang University (0000)</p>
          <a class="person-email">rapael6696@kaist.ac.kr</a>
        </div>
      </article>

       <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/placeholder.png' | relative_url }}" alt="Taeung Lee"></div>
        <div class="person-info">
          <h3 class="person-name">Taeung Lee</h3>
          <p class="person-meta">B.S.: Korea University (0000)</p>
          <a class="person-email">christy201@kaist.ac.kr</a>
        </div>
      </article>

    </div>
  </section>

  <section class="people-section">
    <div class="people-section-title"><h2>Administrator</h2></div>
    <div class="people-grid">
      <article class="person-card">
        <div class="person-photo"><img src="{{ '/assets/img/people/seonah-lee.jpg' | relative_url }}" alt="Seonah Lee"></div>
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
