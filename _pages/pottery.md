---
permalink: /pottery/
title: "Pottery"
layout: default
author_profile: false
---

{% comment %}
One piece per row. Pieces photographed twice sit side by side in one row;
grid columns are proportioned to each photo's aspect ratio so the pair
renders at equal height. Every image ships two WebP sizes via srcset;
the lightbox loads the large one from data-full.
{% endcomment %}

{% capture web %}{{ base_path }}/images/pottery/web{% endcapture %}

<div class="home-wrapper home-wrapper--wide">
  <h1 class="page__title">Pottery</h1>

  <div class="page__content">
    <p> As you can see, I do pottery better than I take photos. </p>
  </div>

  <div class="pot-list">

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-sm" data-full="{{ web }}/01-celadon-vase.webp">
        <img src="{{ web }}/01-celadon-vase-640.webp"
             srcset="{{ web }}/01-celadon-vase-640.webp 640w, {{ web }}/01-celadon-vase.webp 1280w"
             sizes="(max-width: 700px) 94vw, 560px" alt="Celadon bud vase" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-lg" data-full="{{ web }}/02-celadon-bowl.webp">
        <img src="{{ web }}/02-celadon-bowl-640.webp"
             srcset="{{ web }}/02-celadon-bowl-640.webp 640w, {{ web }}/02-celadon-bowl.webp 1280w"
             sizes="(max-width: 900px) 94vw, 860px" alt="Celadon bowl" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--pair" style="grid-template-columns: 1fr 0.8fr;">
      <button type="button" class="gallery-btn" data-full="{{ web }}/03-blush-teabowl-a.webp">
        <img src="{{ web }}/03-blush-teabowl-a-640.webp"
             srcset="{{ web }}/03-blush-teabowl-a-640.webp 640w, {{ web }}/03-blush-teabowl-a.webp 1280w"
             sizes="(max-width: 560px) 94vw, 48vw" alt="Blush tea bowl" loading="lazy" decoding="async">
      </button>
      <button type="button" class="gallery-btn" data-full="{{ web }}/04-blush-teabowl-b.webp">
        <img src="{{ web }}/04-blush-teabowl-b-640.webp"
             srcset="{{ web }}/04-blush-teabowl-b-640.webp 640w, {{ web }}/04-blush-teabowl-b.webp 1280w"
             sizes="(max-width: 560px) 94vw, 40vw" alt="Blush tea bowl, second view" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--pair" style="grid-template-columns: 0.8fr 1fr;">
      <button type="button" class="gallery-btn" data-full="{{ web }}/05-oxblood-tumbler-a.webp">
        <img src="{{ web }}/05-oxblood-tumbler-a-640.webp"
             srcset="{{ web }}/05-oxblood-tumbler-a-640.webp 640w, {{ web }}/05-oxblood-tumbler-a.webp 1280w"
             sizes="(max-width: 560px) 94vw, 40vw" alt="Oxblood tumbler" loading="lazy" decoding="async">
      </button>
      <button type="button" class="gallery-btn" data-full="{{ web }}/06-oxblood-tumbler-b.webp">
        <img src="{{ web }}/06-oxblood-tumbler-b-640.webp"
             srcset="{{ web }}/06-oxblood-tumbler-b-640.webp 640w, {{ web }}/06-oxblood-tumbler-b.webp 1280w"
             sizes="(max-width: 560px) 94vw, 48vw" alt="Oxblood tumbler, second view" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--pair" style="grid-template-columns: 0.8fr 1fr;">
      <button type="button" class="gallery-btn" data-full="{{ web }}/07-faceted-bowl.webp">
        <img src="{{ web }}/07-faceted-bowl-640.webp"
             srcset="{{ web }}/07-faceted-bowl-640.webp 640w, {{ web }}/07-faceted-bowl.webp 1280w"
             sizes="(max-width: 560px) 94vw, 40vw" alt="Faceted maroon bowl" loading="lazy" decoding="async">
      </button>
      <button type="button" class="gallery-btn" data-full="{{ web }}/08-faceted-bowl-interior.webp">
        <img src="{{ web }}/08-faceted-bowl-interior-640.webp"
             srcset="{{ web }}/08-faceted-bowl-interior-640.webp 640w, {{ web }}/08-faceted-bowl-interior.webp 1280w"
             sizes="(max-width: 560px) 94vw, 48vw" alt="Faceted maroon bowl, interior" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-md" data-full="{{ web }}/09-harvest-mug.webp">
        <img src="{{ web }}/09-harvest-mug-640.webp"
             srcset="{{ web }}/09-harvest-mug-640.webp 640w, {{ web }}/09-harvest-mug.webp 1280w"
             sizes="(max-width: 700px) 94vw, 620px" alt="Mug with handle" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-sm" data-full="{{ web }}/10-glacier-tumbler.webp">
        <img src="{{ web }}/10-glacier-tumbler-640.webp"
             srcset="{{ web }}/10-glacier-tumbler-640.webp 640w, {{ web }}/10-glacier-tumbler.webp 1280w"
             sizes="(max-width: 700px) 94vw, 560px" alt="Blue textured tumbler" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-md" data-full="{{ web }}/11-wave-tumbler.webp">
        <img src="{{ web }}/11-wave-tumbler-640.webp"
             srcset="{{ web }}/11-wave-tumbler-640.webp 640w, {{ web }}/11-wave-tumbler.webp 1280w"
             sizes="(max-width: 700px) 94vw, 620px" alt="Blue and white tumbler" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--pair" style="grid-template-columns: 1fr 0.8fr;">
      <button type="button" class="gallery-btn" data-full="{{ web }}/12-tortoise-bowl-a.webp">
        <img src="{{ web }}/12-tortoise-bowl-a-640.webp"
             srcset="{{ web }}/12-tortoise-bowl-a-640.webp 640w, {{ web }}/12-tortoise-bowl-a.webp 1280w"
             sizes="(max-width: 560px) 94vw, 48vw" alt="Tortoiseshell bowl" loading="lazy" decoding="async">
      </button>
      <button type="button" class="gallery-btn" data-full="{{ web }}/13-tortoise-bowl-b.webp">
        <img src="{{ web }}/13-tortoise-bowl-b-640.webp"
             srcset="{{ web }}/13-tortoise-bowl-b-640.webp 640w, {{ web }}/13-tortoise-bowl-b.webp 1280w"
             sizes="(max-width: 560px) 94vw, 40vw" alt="Tortoiseshell bowl, second view" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-lg" data-full="{{ web }}/14-drip-bowl.webp">
        <img src="{{ web }}/14-drip-bowl-640.webp"
             srcset="{{ web }}/14-drip-bowl-640.webp 640w, {{ web }}/14-drip-bowl.webp 1280w"
             sizes="(max-width: 900px) 94vw, 860px" alt="White bowl with amber drips" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-md" data-full="{{ web }}/15-teal-pourer.webp">
        <img src="{{ web }}/15-teal-pourer-640.webp"
             srcset="{{ web }}/15-teal-pourer-640.webp 640w, {{ web }}/15-teal-pourer.webp 1280w"
             sizes="(max-width: 700px) 94vw, 620px" alt="Teal spouted bowl from above" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-lg" data-full="{{ web }}/16-striped-cup-detail.webp">
        <img src="{{ web }}/16-striped-cup-detail-640.webp"
             srcset="{{ web }}/16-striped-cup-detail-640.webp 640w, {{ web }}/16-striped-cup-detail.webp 1280w"
             sizes="(max-width: 900px) 94vw, 860px" alt="Striped cup, detail" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--pair" style="grid-template-columns: 1.6fr 0.8fr;">
      <button type="button" class="gallery-btn" data-full="{{ web }}/17-tipped-cup.webp">
        <img src="{{ web }}/17-tipped-cup-640.webp"
             srcset="{{ web }}/17-tipped-cup-640.webp 640w, {{ web }}/17-tipped-cup.webp 1280w"
             sizes="(max-width: 560px) 94vw, 60vw" alt="Drip-glazed cup on its side" loading="lazy" decoding="async">
      </button>
      <button type="button" class="gallery-btn" data-full="{{ web }}/18-notched-cup.webp">
        <img src="{{ web }}/18-notched-cup-640.webp"
             srcset="{{ web }}/18-notched-cup-640.webp 640w, {{ web }}/18-notched-cup.webp 1280w"
             sizes="(max-width: 560px) 94vw, 30vw" alt="Drip-glazed cup with notched rim" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-md" data-full="{{ web }}/19-speckled-bowl.webp">
        <img src="{{ web }}/19-speckled-bowl-640.webp"
             srcset="{{ web }}/19-speckled-bowl-640.webp 640w, {{ web }}/19-speckled-bowl.webp 1280w"
             sizes="(max-width: 700px) 94vw, 620px" alt="Speckled blue bowl" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-md" data-full="{{ web }}/20-indigo-bowl.webp">
        <img src="{{ web }}/20-indigo-bowl-640.webp"
             srcset="{{ web }}/20-indigo-bowl-640.webp 640w, {{ web }}/20-indigo-bowl.webp 1280w"
             sizes="(max-width: 700px) 94vw, 620px" alt="Indigo bowl" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-sm" data-full="{{ web }}/21-banded-cup.webp">
        <img src="{{ web }}/21-banded-cup-640.webp"
             srcset="{{ web }}/21-banded-cup-640.webp 640w, {{ web }}/21-banded-cup.webp 1280w"
             sizes="(max-width: 700px) 94vw, 560px" alt="Cup with blue band" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-md" data-full="{{ web }}/22-sand-bowl.webp">
        <img src="{{ web }}/22-sand-bowl-640.webp"
             srcset="{{ web }}/22-sand-bowl-640.webp 640w, {{ web }}/22-sand-bowl.webp 1280w"
             sizes="(max-width: 700px) 94vw, 620px" alt="Sand-coloured bowl" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-sm" data-full="{{ web }}/23-amber-tumbler.webp">
        <img src="{{ web }}/23-amber-tumbler-640.webp"
             srcset="{{ web }}/23-amber-tumbler-640.webp 640w, {{ web }}/23-amber-tumbler.webp 1280w"
             sizes="(max-width: 700px) 94vw, 560px" alt="Amber tumbler" loading="lazy" decoding="async">
      </button>
    </div>

    <div class="pot-row pot-row--single">
      <button type="button" class="gallery-btn pot-w-sm" data-full="{{ web }}/24-moss-cup.webp">
        <img src="{{ web }}/24-moss-cup-640.webp"
             srcset="{{ web }}/24-moss-cup-640.webp 640w, {{ web }}/24-moss-cup.webp 1280w"
             sizes="(max-width: 700px) 94vw, 560px" alt="Moss green cup" loading="lazy" decoding="async">
      </button>
    </div>

  </div>
</div>

{% include photo-lightbox.html %}
