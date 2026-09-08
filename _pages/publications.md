---
layout: default
title: Publications
permalink: /publications/
nav: true
nav_order: 4
---

<style>
.publications-page {
  --morin-navy: #0b2d5c;
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

.publications-page h1,
.publications-page h2,
.publications-page h3,
.publications-page p,
.publications-page select {
  font-family: inherit;
}

.publications-page h1 {
  margin: 0 0 12px;
  color: inherit;
  font-size: 2.25rem;
  font-weight: 400;
  line-height: 1.15;
}

.publications-intro {
  max-width: 900px;
  margin: 0 0 28px;
  color: var(--morin-text);
  font-size: 1rem;
  line-height: 1.55;
}

.publications-controls {
  padding: 0 0 20px;
  border-bottom: 1px solid var(--morin-line);
}

.publications-select {
  width: min(360px, 100%);
  padding: 10px 38px 10px 12px;
  border: 1px solid #cfd6df;
  border-radius: 7px;
  background: #fff;
  color: var(--morin-text);
  font-size: .94rem;
  line-height: 1.3;
}

.publications-list {
  border-top: 0;
}

.publication-year {
  margin: 34px 0 0;
  padding: 0 0 7px;
  border-bottom: 2px solid var(--morin-navy);
  color: var(--morin-navy);
  font-size: 1.15rem;
  font-weight: 700;
  line-height: 1.3;
}

.publication-year:first-child {
  margin-top: 4px;
}

.publication-item {
  padding: 17px 0 16px;
  border-bottom: 1px solid var(--morin-line);
}

.publication-title {
  margin: 0 0 5px;
  color: var(--morin-navy);
  font-size: 1rem;
  font-weight: 600;
  line-height: 1.42;
}

.publication-authors {
  margin: 0 0 3px;
  color: var(--morin-text);
  font-size: .89rem;
  line-height: 1.45;
}

.publication-venue {
  margin: 0;
  color: var(--morin-muted);
  font-size: .88rem;
  line-height: 1.45;
  font-style: italic;
}

.publication-count {
  margin: 14px 0 0;
  color: var(--morin-muted);
  font-size: .84rem;
}

.publications-note,
.publication-note {
  color: var(--morin-muted);
  font-size: .86rem;
}

.publication-note {
  margin: 4px 0 0;
  font-style: normal;
}

@media (max-width: 640px) {
  .publications-page {
    width: calc(100% - 30px);
  }
}
</style>

<div class="publications-page">
  <h1>Publications</h1>
  <p class="publications-intro">
    Publications of the Mobile Robotics &amp; Intelligence Laboratory.
    Select a publication type below to view the corresponding list. Publications are sorted by year, newest first.<br>
    <span class="publications-note">* denotes the corresponding author.</span>
  </p>

  <div class="publications-controls">
    <select id="publication-filter" class="publications-select" aria-label="Select publication type">
      <option value="International Journals">International Journals</option>
      <option value="International Conferences">International Conferences</option>
      <option value="Domestic Journals">Domestic Journals</option>
      <option value="Domestic Conferences">Domestic Conferences</option>
    </select>
    <p id="publication-count" class="publication-count"></p>
  </div>

  <div id="publication-list" class="publications-list"></div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  // Publication data lives in _data/publications.yml (single source of truth,
  // shared with the home page's Research Highlights section).
  const publicationData = {{ site.data.publications | jsonify }};
  const select = document.getElementById("publication-filter");
  const list = document.getElementById("publication-list");
  const count = document.getElementById("publication-count");

  function escapeHtml(value) {
    return String(value)
      .replace(/&/g, "&amp;")
      .replace(/</g, "&lt;")
      .replace(/>/g, "&gt;")
      .replace(/"/g, "&quot;")
      .replace(/'/g, "&#039;");
  }

  function render(category) {
    const entries = [...(publicationData[category] || [])].sort((a, b) => Number(b.year) - Number(a.year));
    count.textContent = entries.length + (entries.length === 1 ? " entry" : " entries");

    let currentYear = null;

    list.innerHTML = entries.map(function (item) {
      let heading = "";
      if (item.year !== currentYear) {
        currentYear = item.year;
        heading = `<h2 class="publication-year">${escapeHtml(item.year)}</h2>`;
      }
      return heading + `
        <article class="publication-item">
          <h3 class="publication-title">${escapeHtml(item.title)}</h3>
          <p class="publication-authors">${escapeHtml(item.authors)}</p>
          <p class="publication-venue">${escapeHtml(item.venue)}</p>
          ${item.note ? `<p class="publication-note">${escapeHtml(item.note)}</p>` : ""}
        </article>`;
    }).join("");
  }

  select.addEventListener("change", function () {
    render(this.value);
  });

  render(select.value);
});
</script>
