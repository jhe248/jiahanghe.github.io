---
permalink: /raven/
title: "Raven"
layout: default
author_profile: false
---

{% assign photos = site.static_files | where_exp: "f", "f.path contains '/images/cat/'" | where_exp: "f", "f.extname != '.gitkeep'" | sort: "path" %}

<div class="home-wrapper">
  <h1 class="page__title">Raven</h1>

  <div class="page__content">
    <p>My cat. She supervises most of the writing that happens here.</p>
  </div>

  <div class="gallery" id="gallery">
    {% for photo in photos %}
    <figure class="gallery-item">
      <button type="button" class="gallery-btn" data-index="{{ forloop.index0 }}"
              aria-label="View photo {{ forloop.index }} of {{ photos.size }} larger">
        <img src="{{ base_path }}{{ photo.path }}" alt="Raven, photo {{ forloop.index }}" loading="lazy">
      </button>
    </figure>
    {% endfor %}
  </div>
</div>

<div class="lightbox" id="lightbox" hidden>
  <button type="button" class="lightbox-close" aria-label="Close">&times;</button>
  <button type="button" class="lightbox-nav lightbox-prev" aria-label="Previous photo">&#8249;</button>
  <img class="lightbox-img" id="lightbox-img" src="" alt="">
  <button type="button" class="lightbox-nav lightbox-next" aria-label="Next photo">&#8250;</button>
  <p class="lightbox-count" id="lightbox-count"></p>
</div>

<script>
(function () {
  var buttons = Array.prototype.slice.call(document.querySelectorAll('.gallery-btn'));
  if (!buttons.length) return;

  var box    = document.getElementById('lightbox');
  var img    = document.getElementById('lightbox-img');
  var count  = document.getElementById('lightbox-count');
  var sources = buttons.map(function (b) { return b.querySelector('img'); });
  var current = 0;
  var lastFocused = null;

  function show(i) {
    current = (i + sources.length) % sources.length;
    img.src = sources[current].src;
    img.alt = sources[current].alt;
    count.textContent = (current + 1) + ' / ' + sources.length;
  }

  function open(i) {
    lastFocused = document.activeElement;
    show(i);
    box.hidden = false;
    document.body.style.overflow = 'hidden';
    box.querySelector('.lightbox-close').focus();
  }

  function close() {
    box.hidden = true;
    document.body.style.overflow = '';
    if (lastFocused) lastFocused.focus();
  }

  buttons.forEach(function (b, i) {
    b.addEventListener('click', function () { open(i); });
  });

  box.querySelector('.lightbox-close').addEventListener('click', close);
  box.querySelector('.lightbox-prev').addEventListener('click', function (e) {
    e.stopPropagation(); show(current - 1);
  });
  box.querySelector('.lightbox-next').addEventListener('click', function (e) {
    e.stopPropagation(); show(current + 1);
  });
  box.addEventListener('click', function (e) { if (e.target === box) close(); });

  document.addEventListener('keydown', function (e) {
    if (box.hidden) return;
    if (e.key === 'Escape') close();
    if (e.key === 'ArrowLeft') show(current - 1);
    if (e.key === 'ArrowRight') show(current + 1);
  });
})();
</script>
