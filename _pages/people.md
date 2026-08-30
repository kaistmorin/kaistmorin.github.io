---
layout: page
title: People
permalink: /people/
nav: true
nav_order: 3
---

<style>
.people-page {
  max-width: 1100px;
  margin: 0 auto;
}

.people-page .page-intro {
  margin-bottom: 2.2rem;
  color: #555;
}

.people-section {
  margin-top: 2.8rem;
}

.people-section h2 {
  font-size: 1.6rem;
  font-weight: 700;
  margin-bottom: 1.2rem;
  padding-bottom: 0.4rem;
  border-bottom: 1px solid #e5e5e5;
}

.faculty-card {
  display: grid;
  grid-template-columns: 180px 1fr;
  gap: 1.5rem;
  align-items: center;
  background: #fff;
  border: 1px solid #e8e8e8;
  border-radius: 14px;
  padding: 1.5rem;
  margin-top: 1rem;
}

.people-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.5rem;
  margin-top: 1rem;
}

.person-card {
  background: #fff;
  border: 1px solid #e8e8e8;
  border-radius: 14px;
  padding: 1.25rem;
  text-align: left;
  min-height: 100%;
}

.person-photo-wrap {
  width: 100%;
  display: flex;
  justify-content: center;
  margin-bottom: 1rem;
}

.person-photo {
  width: 180px;
  height: 180px;
  object-fit: cover;
  object-position: center;
  border-radius: 10px;
  background: #f6f6f6;
  border: 1px solid #efefef;
}

.person-name {
  font-size: 1.15rem;
  font-weight: 700;
  margin-bottom: 0.55rem;
}

.person-meta {
  font-size: 0.95rem;
  line-height: 1.65;
  color: #333;
}

.person-meta strong {
  color: #111;
}

.person-email {
  margin-top: 0.8rem;
  font-size: 0.92rem;
  color: #666;
  word-break: break-word;
}

@media (max-width: 900px) {
  .people-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .faculty-card {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .faculty-card .person-photo-wrap {
    justify-content: center;
  }
}

@media (max-width: 640px) {
  .people-grid {
    grid-template-columns: 1fr;
  }

  .person-photo {
    width: 170px;
    height: 170px;
  }
}
</style>

<div class="people-page">

Members of the Mobile Robotics & Intelligence Laboratory at KAIST.

<div class="people-section">
  <h2>Faculty</h2>

  <div class="faculty-card">
    <div class="person-photo-wrap">
      <img class="person-photo" src="/assets/img/people/jinwhan-kim.jpg" alt="Jinwhan Kim">
    </div>
    <div>
      <div class="person-name">Jinwhan Kim</div>
      <div class="person-meta">
        Professor<br>
        Department of Mechanical Engineering, KAIST<br><br>
        <strong>Research:</strong> Autonomous systems, guidance, navigation, control, estimation, and marine robotics
      </div>
      <div class="person-email">jinwhan@kaist.ac.kr</div>
    </div>
  </div>
</div>

<div class="people-section">
  <h2>Postdoctoral Researchers</h2>

  <div class="people-grid">
    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/kyungseo-kim.jpg" alt="Kyungseo Kim">
      </div>
      <div class="person-name">Kyungseo Kim</div>
      <div class="person-meta">
        <strong>Ph.D.:</strong> KAIST
      </div>
      <div class="person-email">chalseokim@kaist.ac.kr</div>
    </div>

    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/jinwook-park.jpg" alt="Jinwook Park">
      </div>
      <div class="person-name">Jinwook Park</div>
      <div class="person-meta">
        <strong>Ph.D.:</strong> KAIST
      </div>
      <div class="person-email">qkrwlsdn10@kaist.ac.kr</div>
    </div>

    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/qianyi-zhang.jpg" alt="Qianyi Zhang">
      </div>
      <div class="person-name">Qianyi Zhang</div>
      <div class="person-meta">
        <strong>Ph.D.:</strong> KAIST
      </div>
      <div class="person-email">qianyizhang@kaist.ac.kr</div>
    </div>
  </div>
</div>

<div class="people-section">
  <h2>Ph.D. Students</h2>

  <div class="people-grid">
    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/sol-han.jpg" alt="Sol Han">
      </div>
      <div class="person-name">Sol Han</div>
      <div class="person-meta">
        <strong>B.S.:</strong> KAIST<br>
        <strong>M.S.:</strong> KAIST
      </div>
      <div class="person-email">[email placeholder]</div>
    </div>

    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/kiyong-park.jpg" alt="Kiyong Park">
      </div>
      <div class="person-name">Kiyong Park</div>
      <div class="person-meta">
        <strong>B.S.:</strong> [placeholder]<br>
        <strong>M.S.:</strong> [placeholder, year]
      </div>
      <div class="person-email">[email placeholder]</div>
    </div>

    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/donghyun-kim.jpg" alt="Donghyun Kim">
      </div>
      <div class="person-name">Donghyun Kim</div>
      <div class="person-meta">
        <strong>B.S.:</strong> [placeholder]<br>
        <strong>M.S.:</strong> [placeholder, year]
      </div>
      <div class="person-email">[email placeholder]</div>
    </div>
  </div>
</div>

<div class="people-section">
  <h2>M.S. Students</h2>

  <div class="people-grid">
    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/student-01.jpg" alt="Student 1">
      </div>
      <div class="person-name">[Name]</div>
      <div class="person-meta">
        <strong>B.S.:</strong> [placeholder]
      </div>
      <div class="person-email">[email placeholder]</div>
    </div>

    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/student-02.jpg" alt="Student 2">
      </div>
      <div class="person-name">[Name]</div>
      <div class="person-meta">
        <strong>B.S.:</strong> [placeholder]
      </div>
      <div class="person-email">[email placeholder]</div>
    </div>

    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/student-03.jpg" alt="Student 3">
      </div>
      <div class="person-name">[Name]</div>
      <div class="person-meta">
        <strong>B.S.:</strong> [placeholder]
      </div>
      <div class="person-email">[email placeholder]</div>
    </div>
  </div>
</div>

<div class="people-section">
  <h2>Administrator</h2>

  <div class="people-grid">
    <div class="person-card">
      <div class="person-photo-wrap">
        <img class="person-photo" src="/assets/img/people/seonah-lee.jpg" alt="Seonah Lee">
      </div>
      <div class="person-name">Seonah Lee</div>
      <div class="person-meta">
        Administrator
      </div>
      <div class="person-email">[email placeholder]</div>
    </div>
  </div>
</div>

</div>