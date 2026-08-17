---
permalink: /pottery/
title: "Pottery"
layout: default
author_profile: false
---

{% assign photos = site.static_files | where_exp: "f", "f.path contains '/images/pottery/web/'" | sort: "path" %}

<div class="home-wrapper home-wrapper--wide">
  <h1 class="page__title">Pottery</h1>

  <div class="page__content">
    <p>I do pottery sometimes. Here is some of my work.</p>
  </div>

  <div class="gallery gallery--three" id="gallery">
    {% for photo in photos %}
    <figure class="gallery-item">
      <button type="button" class="gallery-btn" data-index="{{ forloop.index0 }}"
              aria-label="View photo {{ forloop.index }} of {{ photos.size }} larger">
        <img src="{{ base_path }}{{ photo.path }}" alt="Pottery, photo {{ forloop.index }}" loading="lazy">
      </button>
    </figure>
    {% endfor %}
  </div>
</div>

{% include photo-lightbox.html %}
