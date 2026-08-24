---
permalink: /raven/
title: "Raven"
layout: default
author_profile: false
---

{% assign photos = site.static_files | where_exp: "f", "f.path contains '/images/cat/'" | where_exp: "f", "f.extname != '.gitkeep'" | sort: "path" %}

<div class="home-wrapper home-wrapper--wide">
  <h1 class="page__title">Raven</h1>

  <div class="page__content">
    <p> Raven. She supervises most of the writing that happens here.</p>
  </div>

  <div class="gallery gallery--two" id="gallery">
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

{% include photo-lightbox.html %}
