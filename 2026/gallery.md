---
layout: page-2026
title: "Photos"
permalink: /2026/gallery/
photoswipe: true
---

# 2026 Conference Photos

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
