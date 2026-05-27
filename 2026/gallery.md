---
layout: page-2026
title: "Photos"
permalink: /2026/gallery/
photoswipe: true
---

# Conference Gallery

A selection of photos from the 2026 Applied Machine Learning Conference is available below.

<div class="pswp-gallery gallery-grid" id="gallery">
{% for photo in site.data.gallery-2026 %}
  <a href="https://amlc-images.appliedml.us/2026/{{ photo.filename }}"
     data-pswp-width="2048"
     data-pswp-height="1365">
    <img src="https://amlc-images.appliedml.us/2026/{{ photo.filename }}"
         alt="AMLC 2026">
  </a>
{% endfor %}
</div>

The full photo albums from the 2026 Applied Machine Learning Conference are available on Google Photos. The community album consists of photos taken and contributed by conference attendees.

<div class="gallery-album-links">
  <a href="https://photos.app.goo.gl/983P492hwRpx2eA39" class="btn btn-primary" target="_blank" rel="noopener">View the Official Album</a>
  <a href="https://photos.app.goo.gl/azSfBcQL9jDRx8MeA" class="btn btn-primary" target="_blank" rel="noopener">View the Community Album</a>
</div>
