---
layout: default
title: Events
permalink: /media/events/
nav: false
---

<style>
.media-page,.media-archive,.media-detail{
  --morin-navy:#0b2d5c;
  --morin-text:#1f2937;
  --morin-muted:#667085;
  --morin-line:#e6ebf0;
  width:calc(100% - 48px);
  max-width:1120px;
  box-sizing:border-box;
  margin:0 auto;
  padding:11px 0 72px;
  font-family:inherit;
}
.media-page h1,.media-archive h1,.media-detail h1{
  margin:0 0 12px;font-size:2.25rem;font-weight:400;line-height:1.15;
}
.media-intro{max-width:860px;margin:0 0 30px;color:var(--morin-text);font-size:1rem;line-height:1.55}
.media-section{margin-top:34px}
.media-section-head{display:flex;align-items:center;gap:14px;margin:0 0 15px}
.media-section-head h2{margin:0;color:var(--morin-navy);font-size:1.25rem;font-weight:600}
.media-section-head::after{content:"";flex:1;height:1px;background:var(--morin-line)}
.media-view-all{margin-left:auto;color:var(--morin-navy);font-size:.86rem;font-weight:600;text-decoration:none;white-space:nowrap}
.media-view-all:hover,.archive-back:hover{text-decoration:underline}
.media-featured-video,.media-card,.archive-card{
  overflow:hidden;border:1px solid var(--morin-line);border-radius:8px;background:#fff;
}
.media-video-wrap{position:relative;width:100%;aspect-ratio:16/9;background:#000}
.media-video-wrap iframe{position:absolute;inset:0;width:100%;height:100%;border:0}
.media-featured-meta,.media-card-meta,.archive-meta{padding:12px 13px 14px}
.media-label,.detail-date{margin:0 0 5px;color:var(--morin-muted);font-size:.78rem}
.media-title{margin:0 0 5px;color:var(--morin-navy);font-size:1rem;font-weight:600;line-height:1.4}
.media-desc{margin:0;color:var(--morin-muted);font-size:.88rem;line-height:1.5}
.media-grid,.archive-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:18px}
.media-card a,.archive-card a{display:block;color:inherit;text-decoration:none}
.media-card a:hover .media-title,.archive-card a:hover .media-title{text-decoration:underline;text-underline-offset:2px}
.media-thumb{position:relative;overflow:hidden;aspect-ratio:16/9;background:#f3f5f7}
.media-thumb img{display:block;width:100%;height:100%;object-fit:cover}
.media-play::after{content:"▶";position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);width:42px;height:42px;display:grid;place-items:center;padding-left:3px;border-radius:50%;background:rgba(11,45,92,.88);color:#fff;font-size:15px}
.archive-back{display:inline-block;margin:0 0 20px;color:var(--morin-navy);text-decoration:none;font-size:.9rem}
.archive-grid{margin-top:22px}
.detail-hero{overflow:hidden;border:1px solid var(--morin-line);border-radius:8px;margin:18px 0 24px}
.detail-hero img{display:block;width:100%;max-height:620px;object-fit:cover}
.detail-body{max-width:860px;color:var(--morin-text);font-size:.98rem;line-height:1.7}
.detail-body p{margin:0 0 14px}
.detail-actions{margin-top:18px}
.detail-actions a{color:var(--morin-navy);font-weight:600;text-decoration:none}
.detail-actions a:hover{text-decoration:underline}
@media(max-width:850px){.media-grid,.archive-grid{grid-template-columns:repeat(2,minmax(0,1fr))}}
@media(max-width:640px){.media-page,.media-archive,.media-detail{width:calc(100% - 30px)}.media-grid,.archive-grid{grid-template-columns:1fr}}
</style>

<div class="media-archive">
  <a class="archive-back" href="{{ '/media/' | relative_url }}">← Back to Media</a>
  <h1>Events</h1>
  <p class="media-intro">Awards, conference activities, workshops, competitions, and other notable MORIN Lab events.</p>
  <div class="archive-grid">
  <article class="archive-card">
    <a href="{{ '/media/events/2026-07-15-dongwook-lee-best-application-paper-award-candidate-at-ur-2026/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-01.jpg' | relative_url }}" alt="Dongwook Lee — Best Application Paper Award Candidate at UR 2026"></div>
      <div class="archive-meta">
        <p class="media-label">2026-07-15</p>
        <h3 class="media-title">Dongwook Lee — Best Application Paper Award Candidate at UR 2026</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2026-07-02-taekjoong-kwon-best-paper-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-02.jpg' | relative_url }}" alt="Taekjoong Kwon — Best Paper Award"></div>
      <div class="archive-meta">
        <p class="media-label">2026-07-02</p>
        <h3 class="media-title">Taekjoong Kwon — Best Paper Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2025-11-11-taekjoong-kwon-and-jinwhan-kim-encouragement-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-03.jpg' | relative_url }}" alt="Taekjoong Kwon and Jinwhan Kim — Encouragement Award"></div>
      <div class="archive-meta">
        <p class="media-label">2025-11-11</p>
        <h3 class="media-title">Taekjoong Kwon and Jinwhan Kim — Encouragement Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2025-09-29-taewoo-lee-student-excellent-poster-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-04.jpg' | relative_url }}" alt="Taewoo Lee — Student Excellent Poster Award"></div>
      <div class="archive-meta">
        <p class="media-label">2025-09-29</p>
        <h3 class="media-title">Taewoo Lee — Student Excellent Poster Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2025-06-18-dongwook-lee-third-prize-at-oceans-25-student-poster-competition/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-05.jpg' | relative_url }}" alt="Dongwook Lee — Third Prize at OCEANS&#x27;25 Student Poster Competition"></div>
      <div class="archive-meta">
        <p class="media-label">2025-06-18</p>
        <h3 class="media-title">Dongwook Lee — Third Prize at OCEANS'25 Student Poster Competition</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2024-05-23-dongha-chung-grand-prize-at-kaosts-paper-contest/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-06.jpg' | relative_url }}" alt="Dongha Chung — Grand Prize at KAOSTS Paper Contest"></div>
      <div class="archive-meta">
        <p class="media-label">2024-05-23</p>
        <h3 class="media-title">Dongha Chung — Grand Prize at KAOSTS Paper Contest</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2024-04-17-qianyi-zhang-oceans-24-student-poster-competition/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-07.jpg' | relative_url }}" alt="Qianyi Zhang — OCEANS&#x27;24 Student Poster Competition"></div>
      <div class="archive-meta">
        <p class="media-label">2024-04-17</p>
        <h3 class="media-title">Qianyi Zhang — OCEANS'24 Student Poster Competition</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2024-02-01-team-kaist-2nd-place-winner-in-mbzirc-2023/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-08.jpg' | relative_url }}" alt="Team KAIST — 2nd Place Winner in MBZIRC 2023"></div>
      <div class="archive-meta">
        <p class="media-label">2024-02-01</p>
        <h3 class="media-title">Team KAIST — 2nd Place Winner in MBZIRC 2023</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2024-02-23-eunghyun-kim-most-outstanding-paper-award-at-kroc-2024/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-09.jpg' | relative_url }}" alt="Eunghyun Kim — Most Outstanding Paper Award at KRoC 2024"></div>
      <div class="archive-meta">
        <p class="media-label">2024-02-23</p>
        <h3 class="media-title">Eunghyun Kim — Most Outstanding Paper Award at KRoC 2024</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2023-06-08-donghyun-kim-oceans-23-student-poster-competition/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-10.jpg' | relative_url }}" alt="Donghyun Kim — OCEANS&#x27;23 Student Poster Competition"></div>
      <div class="archive-meta">
        <p class="media-label">2023-06-08</p>
        <h3 class="media-title">Donghyun Kim — OCEANS'23 Student Poster Competition</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2022-06-23-kyungseo-kim-outstanding-paper-award-at-icros-2022/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-11.jpg' | relative_url }}" alt="Kyungseo Kim — Outstanding Paper Award at ICROS 2022"></div>
      <div class="archive-meta">
        <p class="media-label">2022-06-23</p>
        <h3 class="media-title">Kyungseo Kim — Outstanding Paper Award at ICROS 2022</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2022-05-13-sol-han-and-jungwoo-han-outstanding-paper-award-at-kroc-2022/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-12.jpg' | relative_url }}" alt="Sol Han and Jungwoo Han — Outstanding Paper Award at KRoC 2022"></div>
      <div class="archive-meta">
        <p class="media-label">2022-05-13</p>
        <h3 class="media-title">Sol Han and Jungwoo Han — Outstanding Paper Award at KRoC 2022</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2022-01-18-jonghwi-kim-outstanding-student-paper-presentation-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-13.jpg' | relative_url }}" alt="Jonghwi Kim — Outstanding Student Paper Presentation Award"></div>
      <div class="archive-meta">
        <p class="media-label">2022-01-18</p>
        <h3 class="media-title">Jonghwi Kim — Outstanding Student Paper Presentation Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2021-01-21-junwoo-jang-outstanding-student-paper-presentation-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-14.jpg' | relative_url }}" alt="Junwoo Jang — Outstanding Student Paper Presentation Award"></div>
      <div class="archive-meta">
        <p class="media-label">2021-01-21</p>
        <h3 class="media-title">Junwoo Jang — Outstanding Student Paper Presentation Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2020-12-03-changyu-lee-outstanding-student-paper-presentation-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-15.jpg' | relative_url }}" alt="Changyu Lee — Outstanding Student Paper Presentation Award"></div>
      <div class="archive-meta">
        <p class="media-label">2020-12-03</p>
        <h3 class="media-title">Changyu Lee — Outstanding Student Paper Presentation Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2020-07-03-korean-federation-of-science-technology-societies-best-paper-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-16.jpg' | relative_url }}" alt="Korean Federation of Science &amp; Technology Societies Best Paper Award"></div>
      <div class="archive-meta">
        <p class="media-label">2020-07-03</p>
        <h3 class="media-title">Korean Federation of Science & Technology Societies Best Paper Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2019-12-06-virtual-robotx-vrx-competition-1st-place/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-17.jpg' | relative_url }}" alt="Virtual RobotX (VRX) Competition — 1st Place"></div>
      <div class="archive-meta">
        <p class="media-label">2019-12-06</p>
        <h3 class="media-title">Virtual RobotX (VRX) Competition — 1st Place</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2019-07-26-morin-hero-joint-summer-workshop/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-18.jpg' | relative_url }}" alt="MORIN-HERO Joint Summer Workshop"></div>
      <div class="archive-meta">
        <p class="media-label">2019-07-26</p>
        <h3 class="media-title">MORIN-HERO Joint Summer Workshop</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2019-06-20-keunhwan-kim-oceans-19-student-poster-competition/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-19.jpg' | relative_url }}" alt="Keunhwan Kim — OCEANS&#x27;19 Student Poster Competition"></div>
      <div class="archive-meta">
        <p class="media-label">2019-06-20</p>
        <h3 class="media-title">Keunhwan Kim — OCEANS'19 Student Poster Competition</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2019-04-19-junwoo-jang-excellence-prize-at-ut-19/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-20.jpg' | relative_url }}" alt="Junwoo Jang — Excellence Prize at UT&#x27;19"></div>
      <div class="archive-meta">
        <p class="media-label">2019-04-19</p>
        <h3 class="media-title">Junwoo Jang — Excellence Prize at UT'19</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2018-11-28-morin-winter-workshop/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-21.jpg' | relative_url }}" alt="MORIN Winter Workshop"></div>
      <div class="archive-meta">
        <p class="media-label">2018-11-28</p>
        <h3 class="media-title">MORIN Winter Workshop</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2018-09-21-junwoo-jang-poster-presentation-award-2nd-place/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-22.jpg' | relative_url }}" alt="Junwoo Jang — Poster Presentation Award, 2nd Place"></div>
      <div class="archive-meta">
        <p class="media-label">2018-09-21</p>
        <h3 class="media-title">Junwoo Jang — Poster Presentation Award, 2nd Place</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2017-12-15-jungwook-han-and-yonghoon-cho-best-paper-award-at-maritime-robotx-foru/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-23.jpg' | relative_url }}" alt="Jungwook Han and Yonghoon Cho — Best Paper Award at Maritime RobotX Forum"></div>
      <div class="archive-meta">
        <p class="media-label">2017-12-15</p>
        <h3 class="media-title">Jungwook Han and Yonghoon Cho — Best Paper Award at Maritime RobotX Forum</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2017-09-01-taeyun-kim-and-seonghun-hong-oceans-17-student-poster-competition/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-24.jpg' | relative_url }}" alt="Taeyun Kim and Seonghun Hong — OCEANS&#x27;17 Student Poster Competition"></div>
      <div class="archive-meta">
        <p class="media-label">2017-09-01</p>
        <h3 class="media-title">Taeyun Kim and Seonghun Hong — OCEANS'17 Student Poster Competition</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2017-05-04-sukmin-yoon-outstanding-paper-award-at-icros/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-25.jpg' | relative_url }}" alt="Sukmin Yoon — Outstanding Paper Award at ICROS"></div>
      <div class="archive-meta">
        <p class="media-label">2017-05-04</p>
        <h3 class="media-title">Sukmin Yoon — Outstanding Paper Award at ICROS</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2017-05-04-morin-spring-hiking/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-26.jpg' | relative_url }}" alt="MORIN Spring Hiking"></div>
      <div class="archive-meta">
        <p class="media-label">2017-05-04</p>
        <h3 class="media-title">MORIN Spring Hiking</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2017-04-20-seonghun-hong-grand-prize-at-kaosts-paper-contest/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-27.jpg' | relative_url }}" alt="Seonghun Hong — Grand Prize at KAOSTS Paper Contest"></div>
      <div class="archive-meta">
        <p class="media-label">2017-04-20</p>
        <h3 class="media-title">Seonghun Hong — Grand Prize at KAOSTS Paper Contest</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2017-02-24-taeyun-kim-1st-prize-at-ut-2017-student-poster-competition/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-28.jpg' | relative_url }}" alt="Taeyun Kim — 1st Prize at UT 2017 Student Poster Competition"></div>
      <div class="archive-meta">
        <p class="media-label">2017-02-24</p>
        <h3 class="media-title">Taeyun Kim — 1st Prize at UT 2017 Student Poster Competition</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2017-02-07-jeonghyeon-wang-best-robot-vision-paper-award-at-kroc-2017/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-29.jpg' | relative_url }}" alt="Jeonghyeon Wang — Best Robot Vision Paper Award at KRoC 2017"></div>
      <div class="archive-meta">
        <p class="media-label">2017-02-07</p>
        <h3 class="media-title">Jeonghyeon Wang — Best Robot Vision Paper Award at KRoC 2017</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2017-02-06-morin-winter-workshop/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-30.jpg' | relative_url }}" alt="MORIN Winter Workshop"></div>
      <div class="archive-meta">
        <p class="media-label">2017-02-06</p>
        <h3 class="media-title">MORIN Winter Workshop</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2017-02-03-seonghun-hong-outstanding-student-paper-award-from-ksoe-2016/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-31.jpg' | relative_url }}" alt="Seonghun Hong — Outstanding Student Paper Award from KSOE 2016"></div>
      <div class="archive-meta">
        <p class="media-label">2017-02-03</p>
        <h3 class="media-title">Seonghun Hong — Outstanding Student Paper Award from KSOE 2016</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2016-11-17-dongha-chung-outstanding-student-paper-presentation/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-32.jpg' | relative_url }}" alt="Dongha Chung — Outstanding Student Paper Presentation"></div>
      <div class="archive-meta">
        <p class="media-label">2016-11-17</p>
        <h3 class="media-title">Dongha Chung — Outstanding Student Paper Presentation</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2016-04-13-jungwook-han-third-prize-at-oceans-16-student-poster-competition/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-33.jpg' | relative_url }}" alt="Jungwook Han — Third Prize at OCEANS&#x27;16 Student Poster Competition"></div>
      <div class="archive-meta">
        <p class="media-label">2016-04-13</p>
        <h3 class="media-title">Jungwook Han — Third Prize at OCEANS'16 Student Poster Competition</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2016-01-27-jisung-park-afcv-best-robot-vision-paper-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-34.jpg' | relative_url }}" alt="Jisung Park — AFCV Best Robot Vision Paper Award"></div>
      <div class="archive-meta">
        <p class="media-label">2016-01-27</p>
        <h3 class="media-title">Jisung Park — AFCV Best Robot Vision Paper Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2016-01-26-minju-kang-outstanding-student-poster-award-at-kroc/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-35.jpg' | relative_url }}" alt="Minju Kang — Outstanding Student Poster Award at KRoC"></div>
      <div class="archive-meta">
        <p class="media-label">2016-01-26</p>
        <h3 class="media-title">Minju Kang — Outstanding Student Poster Award at KRoC</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2016-01-26-morin-winter-workshop/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-36.jpg' | relative_url }}" alt="MORIN Winter Workshop"></div>
      <div class="archive-meta">
        <p class="media-label">2016-01-26</p>
        <h3 class="media-title">MORIN Winter Workshop</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2015-10-22-jeonghyeon-wang-outstanding-student-paper-award-from-ksoe/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-37.jpg' | relative_url }}" alt="Jeonghyeon Wang — Outstanding Student Paper Award from KSOE"></div>
      <div class="archive-meta">
        <p class="media-label">2015-10-22</p>
        <h3 class="media-title">Jeonghyeon Wang — Outstanding Student Paper Award from KSOE</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2015-10-29-seonghun-hong-best-paper-award-from-jkros/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-38.jpg' | relative_url }}" alt="Seonghun Hong — Best Paper Award from JKROS"></div>
      <div class="archive-meta">
        <p class="media-label">2015-10-29</p>
        <h3 class="media-title">Seonghun Hong — Best Paper Award from JKROS</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2015-05-07-sungchur-kwon-outstanding-poster-award-at-kroc-2015/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-39.jpg' | relative_url }}" alt="Sungchur Kwon — Outstanding Poster Award at KRoC 2015"></div>
      <div class="archive-meta">
        <p class="media-label">2015-05-07</p>
        <h3 class="media-title">Sungchur Kwon — Outstanding Poster Award at KRoC 2015</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2014-10-26-robotx-competition-2nd-place/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-40.jpg' | relative_url }}" alt="RobotX Competition — 2nd Place"></div>
      <div class="archive-meta">
        <p class="media-label">2014-10-26</p>
        <h3 class="media-title">RobotX Competition — 2nd Place</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2014-05-23-jisung-park-outstanding-student-paper-presentation-award/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-41.jpg' | relative_url }}" alt="Jisung Park — Outstanding Student Paper &amp; Presentation Award"></div>
      <div class="archive-meta">
        <p class="media-label">2014-05-23</p>
        <h3 class="media-title">Jisung Park — Outstanding Student Paper & Presentation Award</h3>
      </div>
    </a>
  </article>
  <article class="archive-card">
    <a href="{{ '/media/events/2014-01-28-jungwook-han-outstanding-paper-award-from-ksoe/' | relative_url }}">
      <div class="media-thumb"><img src="{{ '/assets/img/media/events/event-42.jpg' | relative_url }}" alt="Jungwook Han — Outstanding Paper Award from KSOE"></div>
      <div class="archive-meta">
        <p class="media-label">2014-01-28</p>
        <h3 class="media-title">Jungwook Han — Outstanding Paper Award from KSOE</h3>
      </div>
    </a>
  </article></div>
</div>
