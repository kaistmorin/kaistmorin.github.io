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
  --morin-sky: #1f8fd0;
  --morin-sky-soft: #a8d8f2;
  --morin-sky-tint: #eaf5fc;
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

.publications-filters {
  display: flex;
  flex-wrap: wrap;
  gap: 14px 16px;
}

.publications-field {
  display: flex;
  flex-direction: column;
  gap: 6px;
  min-width: 0;
}

.publications-field--type { width: min(245px, 100%); }
.publications-field--area { width: min(155px, 100%); }
.publications-field--year { width: min(135px, 100%); }
.publications-field--author { width: min(255px, 100%); }

.publications-field-label {
  color: var(--morin-muted);
  font-size: .76rem;
  font-weight: 600;
  letter-spacing: .05em;
  text-transform: uppercase;
}

.publications-select {
  width: 100%;
  padding: 10px 32px 10px 12px;
  border: 1px solid #cfd6df;
  border-radius: 7px;
  background: #fff;
  color: var(--morin-text);
  font-size: .94rem;
  line-height: 1.3;
  /* overrides the theme's magenta highlight on the open dropdown */
  accent-color: var(--morin-sky);
}

.publications-select:hover {
  border-color: var(--morin-sky-soft);
}

/* !important: the theme's own focus colour is magenta and lives in a gem-owned
   stylesheet this repo must not edit, so it has to be beaten here. */
.publications-select:focus,
.publications-select:focus-visible {
  border-color: var(--morin-sky) !important;
  outline: 2px solid var(--morin-sky-soft) !important;
  outline-offset: 1px;
  box-shadow: 0 0 0 3px rgba(31, 143, 208, .20) !important;
}

.publications-select option:checked,
.publications-select option:hover {
  background: var(--morin-sky) !important;
  color: #fff !important;
}

.publication-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
  margin: 8px 0 0;
}

.publication-category,
.publication-area {
  display: inline-block;
  padding: 2px 8px;
  border-radius: 4px;
  font-size: .74rem;
  font-weight: 600;
  letter-spacing: .02em;
}

.publication-category {
  background: #f3f4f6;
  color: #4b5563;
}

/* One colour per research area, reused by the badge and the filter legend. */
.publication-area--perception {
  background: #e2f1f8;
  color: #0f6f92;
  box-shadow: inset 0 0 0 1px #bfdfed;
}

.publication-area--planning {
  background: #fbeedd;
  color: #99590a;
  box-shadow: inset 0 0 0 1px #f0d7b4;
}

.publication-area--control {
  background: #ece6fa;
  color: #5c42ab;
  box-shadow: inset 0 0 0 1px #d5c9f2;
}

.publications-empty {
  margin: 26px 0 0;
  color: var(--morin-muted);
  font-size: .95rem;
}

.publications-list {
  border-top: 0;
}

.publication-year {
  margin: 34px 0 0;
  padding: 0 0 7px;
  border-bottom: 2px solid var(--morin-sky-soft);
  color: var(--morin-sky);
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
    Filter by type, research area, year or author. Publications are sorted by year, newest first.<br>
    <span class="publications-note">* denotes the corresponding author.</span>
  </p>

  <div class="publications-controls">
    <div class="publications-filters">
      <label class="publications-field publications-field--type">
        <span class="publications-field-label">Type</span>
        <select id="publication-filter" class="publications-select">
          <option value="">All Types</option>
          <option value="International Journals" selected>International Journals</option>
          <option value="International Conferences">International Conferences</option>
          <option value="Domestic Journals">Domestic Journals</option>
          <option value="Domestic Conferences">Domestic Conferences</option>
        </select>
      </label>
      <label class="publications-field publications-field--area">
        <span class="publications-field-label">Area</span>
        <select id="publication-area-filter" class="publications-select"></select>
      </label>
      <label class="publications-field publications-field--year">
        <span class="publications-field-label">Year</span>
        <select id="publication-year-filter" class="publications-select"></select>
      </label>
      <label class="publications-field publications-field--author">
        <span class="publications-field-label">Author</span>
        <select id="publication-author-filter" class="publications-select"></select>
      </label>
    </div>
    <p id="publication-count" class="publication-count"></p>
  </div>

  <div id="publication-list" class="publications-list"></div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  // Publication data lives in _data/publications.yml (single source of truth,
  // shared with the home page's Research Highlights section).
  const publicationData = {{ site.data.publications | jsonify }};
  // Author filter roster: lab members only, Korean and English spellings merged.
  const authorRoster = {{ site.data.publication_authors | jsonify }};
  const catSelect = document.getElementById("publication-filter");
  const areaSelect = document.getElementById("publication-area-filter");
  const yearSelect = document.getElementById("publication-year-filter");
  const authorSelect = document.getElementById("publication-author-filter");
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

  // Ignore case, spaces, hyphens and periods when matching a spelling.
  function normalizeName(value) {
    return String(value || "").replace(/[\s\-.]/g, "").toLowerCase();
  }

  // spelling -> canonical member name, plus the "English (한글)" label to show.
  const authorLookup = new Map();
  const authorLabel = new Map();
  authorRoster.forEach(function (person) {
    authorLabel.set(person.name, person.korean ? person.name + " (" + person.korean + ")" : person.name);
    [person.name].concat(person.korean || [], person.aliases || []).forEach(function (spelling) {
      authorLookup.set(normalizeName(spelling), person.name);
    });
  });

  // "Hakmo Son, Haggi Do and Jinwhan Kim*" -> canonical member names only;
  // co-authors from outside the lab are deliberately left out of the filter.
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

  // Flatten every category once, tagging each entry with the category it came from.
  const entriesAll = [];
  Object.keys(publicationData).forEach(function (category) {
    (publicationData[category] || []).forEach(function (item) {
      entriesAll.push({
        category: category,
        title: item.title,
        authors: item.authors,
        authorList: memberAuthors(item.authors),
        venue: item.venue,
        year: item.year,
        area: item.area || "",
        note: item.note
      });
    });
  });

  function selectEntries(category, area, year, author) {
    return entriesAll.filter(function (item) {
      return (!category || item.category === category)
        && (!area || item.area === area)
        && (!year || item.year === year)
        && (!author || item.authorList.indexOf(author) !== -1);
    });
  }

  // Fixed order so the areas always read perception -> planning -> control.
  const AREA_ORDER = ["Perception", "Planning", "Control"];

  function areaOptions(entries) {
    const present = {};
    entries.forEach(function (item) { if (item.area) present[item.area] = true; });
    return AREA_ORDER.filter(function (a) { return present[a]; })
      .map(function (a) { return { value: a, label: a }; });
  }

  function areaClass(area) {
    return area ? "publication-area publication-area--" + area.toLowerCase() : "";
  }

  // Rebuild a select, keeping the current choice when it is still available.
  function fillSelect(select, options, allLabel) {
    const wanted = select.value;
    const keep = options.some(function (o) { return o.value === wanted; }) ? wanted : "";
    select.innerHTML = '<option value="">' + escapeHtml(allLabel) + "</option>"
      + options.map(function (o) {
          return '<option value="' + escapeHtml(o.value) + '">' + escapeHtml(o.label) + "</option>";
        }).join("");
    select.value = keep;
    return keep;
  }

  function yearOptions(entries) {
    const years = [];
    entries.forEach(function (item) {
      if (years.indexOf(item.year) === -1) years.push(item.year);
    });
    years.sort(function (a, b) { return Number(b) - Number(a); });
    return years.map(function (y) { return { value: y, label: y }; });
  }

  function authorOptions(entries) {
    const tally = new Map();
    entries.forEach(function (item) {
      item.authorList.forEach(function (name) {
        tally.set(name, (tally.get(name) || 0) + 1);
      });
    });
    return Array.from(tally.keys())
      .sort(function (a, b) { return a.localeCompare(b, "en"); })
      .map(function (name) {
        return { value: name, label: (authorLabel.get(name) || name) + " · " + tally.get(name) };
      });
  }

  function render(entries, showCategory) {
    const sorted = entries.slice().sort(function (a, b) { return Number(b.year) - Number(a.year); });
    count.textContent = sorted.length + (sorted.length === 1 ? " entry" : " entries");

    if (!sorted.length) {
      list.innerHTML = '<p class="publications-empty">No publications match the selected filters.</p>';
      return;
    }

    let currentYear = null;

    list.innerHTML = sorted.map(function (item) {
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
          ${item.area || showCategory ? `<div class="publication-tags">
            ${item.area ? `<span class="${areaClass(item.area)}">${escapeHtml(item.area)}</span>` : ""}
            ${showCategory ? `<span class="publication-category">${escapeHtml(item.category)}</span>` : ""}
          </div>` : ""}
        </article>`;
    }).join("");
  }

  // Year options follow type + author, author options follow type + year, so the
  // three filters can never combine into an empty result.
  function update() {
    const category = catSelect.value;
    const area = fillSelect(areaSelect,
      areaOptions(selectEntries(category, "", yearSelect.value, authorSelect.value)), "All Areas");
    const year = fillSelect(yearSelect,
      yearOptions(selectEntries(category, area, "", authorSelect.value)), "All Years");
    const author = fillSelect(authorSelect,
      authorOptions(selectEntries(category, area, year, "")), "All Authors");
    render(selectEntries(category, area, year, author), !category);
  }

  [catSelect, areaSelect, yearSelect, authorSelect].forEach(function (el) {
    el.addEventListener("change", update);
  });

  // Deep links: /publications/?author=Sol%20Han (also &type=, &area=, &year=).
  // The People page links here so one member's papers can be browsed in full;
  // asking for an author without a type widens the type filter to All Types.
  // A select that is filled by update() needs a placeholder option first, or
  // assigning its value would not stick.
  function preselect(select, value) {
    if (!value) return;
    select.innerHTML = '<option value="' + escapeHtml(value) + '"></option>';
    select.value = value;
  }

  const params = new URLSearchParams(window.location.search);
  const wantedType = params.get("type");
  const wantedAuthor = params.get("author");
  if (wantedType !== null) catSelect.value = wantedType;
  else if (wantedAuthor) catSelect.value = "";
  preselect(areaSelect, params.get("area"));
  preselect(yearSelect, params.get("year"));
  preselect(authorSelect, wantedAuthor);

  update();
});
</script>
