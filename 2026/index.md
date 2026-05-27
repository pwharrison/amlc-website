---
layout: home-2026
permalink: /2026/
year: 2026
photoswipe: true
---

<div class="hero">
  <div class="hero-content">
    <div class="hero-logo">
      <img src="{{ '/assets/images/amlc-hero-logo.svg' | relative_url }}" alt="Applied Machine Learning Conference">
    </div>
    <p class="hero-date">April 17-18, 2026</p>
    <p class="hero-subtitle">Charlottesville, Virginia</p>
    <div class="hero-cta">
      <a href="{{ '/2026/gallery/' | relative_url }}" class="btn btn-primary">View the Gallery</a>
      <a href="{{ '/2026/schedule/' | relative_url }}" class="btn btn-primary">View Sessions and Recordings</a>
    </div>
  </div>
</div>

<section class="about">
  <div class="container">
    <h2>About the Conference</h2>
    <p>The Applied Machine Learning Conference is a two-day, in-person event that brings together data scientists, AI engineers, computational researchers, and other technical leaders from across the country to share knowledge, learn from each other, and advance the fields of applied machine learning, AI, and scientific computing.</p>
    <p>The first day of the conference will feature keynotes, standard conference talks, and plentiful networking opportunities, while day two will be filled with practical, 90-minute tutorials diving deeper into the latest tools and techniques used by modern data science and AI professionals.
    </p>
  </div>
</section>

<section class="highlights">
  <div class="container">
    <div class="highlights-grid">
      <div class="highlight-item">
        <h3>Technical Talks</h3>
        <p>Learn from industry experts and academic researchers about the latest developments in data science and AI.</p>
      </div>
      <div class="highlight-item">
        <h3>Practical Tutorials</h3>
        <p>Participate in hands-on sessions to build your skills and learn new tools and techniques.</p>
      </div>
      <div class="highlight-item">
        <h3>Networking</h3>
        <p>Connect with fellow practitioners, share experiences, and build lasting professional relationships.</p>
      </div>
    </div>
  </div>
</section>

<section class="venues">
  <div class="container">
    <h2>Dates and Venues</h2>
    <div class="venue-item">
      <img src="{{ '/assets/images/venue-day1.jpg' | relative_url }}" alt="Violet Crown Charlottesville">
      <div class="venue-info">
        <h3>Friday, April 17: Keynotes, Technical Talks, and Networking</h3>
        <p><b>Violet Crown Cinema</b></p>
        <p><i>200 West Main Street</i></p>
        <p><i>Charlottesville, VA 22902</i></p>
      </div>
    </div>
    <div class="venue-item">
      <img src="{{ '/assets/images/venue-day2.jpg' | relative_url }}" alt="UVA School of Data Science">
      <div class="venue-info">
        <h3>Saturday, April 18: Practical Tutorials and Lightning Talks</h3>
        <p><b>UVA School of Data Science</b></p>
        <p><i>1919 Ivy Road</i></p>
        <p><i>Charlottesville, VA 22904</i></p>
      </div>
    </div>
  </div>
</section>

<section class="featured-speaker">
  <div class="container">
    <h2>Keynote Speakers</h2>
    <div class="speaker-cards">
      <div class="speaker-card">
        <a href="/2026/sessions/keynote-build-yourself-flowers/">
          <div class="speaker-headshot">
            <img src="{{ '/assets/images/vicki-boykis.png' | relative_url }}" alt="Vicki Boykis">
          </div>
          <span class="speaker-name-row">
            <span class="speaker-name">Vicki Boykis</span>
          </span>
          <span class="speaker-tagline">Founding ML Engineer, Malachyte</span>
        </a>
      </div>
      <div class="speaker-card">
        <a href="/2026/sessions/keynote-graphics-ai-and-the-quest-for-new-experiences-at-nvidia/">
          <div class="speaker-headshot">
            <img src="{{ '/assets/images/david-luebke.png' | relative_url }}" alt="David Luebke">
          </div>
          <span class="speaker-name-row">
            <span class="speaker-name">David Luebke</span>
          </span>
          <span class="speaker-tagline">Co-founder of NVIDIA Research</span>
        </a>
      </div>
    </div>
  </div>
</section>

<section class="speaker-wall">
  <div class="container">
    <h2>Featured Speakers</h2>
    <div class="speaker-wall-grid">
      {% include speaker-wall-2026.html %}
    </div>
  </div>
</section>

<section class="featured-photos">
  <div class="container">
    <h2>Selected Photos</h2>
    <div class="pswp-gallery gallery-grid" id="featured-gallery">
      {% assign featured_photos = site.data.gallery-2026 | where: "featured", true %}
      {% for photo in featured_photos %}
      <a href="https://amlc-images.appliedml.us/2026/{{ photo.filename }}"
         data-pswp-width="2048"
         data-pswp-height="1365">
        <img src="https://amlc-images.appliedml.us/2026/{{ photo.filename }}"
             alt="AMLC 2026">
      </a>
      {% endfor %}
    </div>
    <div style="text-align: center; margin-top: var(--spacing-xl);">
      <a href="{{ '/2026/gallery/' | relative_url }}" class="btn btn-primary">View the Gallery</a>
    </div>
  </div>
</section>

<section class="sponsors">
  <div class="container">
    <h2>Thank You to Our Sponsors</h2>
    <h3>Diamond</h3>
    <div class="sponsor-logos sponsor-tier-diamond">
      <div class="sponsor-item">
        <img src="{{ '/assets/images/sponsor-uva-data-science.svg' | relative_url }}" alt="UVA Data Science">
        <span class="sponsor-label">Event Host</span>
      </div>
      <img src="{{ '/assets/images/sponsor-sp-global.svg' | relative_url }}" alt="S&P Global">
    </div>
    <h3>Platinum</h3>
    <div class="sponsor-logos sponsor-tier-platinum">
      <img src="{{ '/assets/images/sponsor-ga-intelligence.svg' | relative_url }}" alt="GA-Intelligence">
    </div>
    <h3>Gold</h3>
    <div class="sponsor-logos sponsor-tier-gold">
      <img src="{{ '/assets/images/sponsor-lacross-ai-institute.png' | relative_url }}" alt="LaCross AI Institute">
      <img src="{{ '/assets/images/sponsor-rotational-labs.svg' | relative_url }}" alt="Rotational Labs">
    </div>
  </div>
</section>
