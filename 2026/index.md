---
layout: home-2026
permalink: /2026/
year: 2026
---

<div class="hero">
  <div class="hero-content">
    <div class="hero-logo">
      <img src="{{ '/assets/images/amlc-hero-logo.svg' | relative_url }}" alt="Applied Machine Learning Conference">
    </div>
    <p class="hero-date">April 17-18, 2026</p>
    <p class="hero-subtitle">Charlottesville, Virginia</p>
    <div class="hero-cta">
      <a href="{{ '/2026/cfp/' | relative_url }}" class="btn btn-primary">Submit a Proposal</a>
      <a href="{{ '/2026/register/' | relative_url }}" class="btn btn-primary">Buy Tickets</a>
      <a href="{{ '/2026/sponsors/' | relative_url }}" class="btn btn-primary">Become a Sponsor</a>
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

<section class="featured-speaker">
  <div class="container">
    <h2>Keynote Speaker</h2>
    <details class="speaker-card">
      <summary class="speaker-summary">
        <div class="speaker-headshot">
          <img src="{{ '/assets/images/vicki-boykis.png' | relative_url }}" alt="Vicki Boykis">
        </div>
        <span class="speaker-name-row">
          <svg class="speaker-chevron" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
            <polyline points="9 6 15 12 9 18"></polyline>
          </svg>
          <span class="speaker-name">Vicki Boykis</span>
        </span>
      </summary>
      <div class="speaker-bio">
        <p><i>Vicki is a founding ML engineer at Malachyte. Previously, she built LLM-evaluation tooling at Mozilla.ai and search/recommendation systems at Duo and Tumblr. She writes about scalable ML in production, information retrieval, and human-centric AI. She previously organized NormConf, a conference about everyday machine learning. She keynoted PyData Amsterdam and PyCon Italia. In her "free time", she writes short stories, learns to DJ by making terrible mixes and loves Nutella.</i></p>
      </div>
    </details>
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
        <h3>Saturday, April 18: Practical Tutorials</h3>
        <p><b>UVA School of Data Science</b></p>
        <p><i>1919 Ivy Road</i></p>
        <p><i>Charlottesville, VA 22904</i></p>
      </div>
    </div>
  </div>
</section>

<script>
  (function() {
    var card = document.querySelector('.speaker-card');
    if (!card) return;
    var bio = card.querySelector('.speaker-bio');
    var summary = card.querySelector('.speaker-summary');

    summary.addEventListener('click', function(e) {
      e.preventDefault();
      if (card.open) {
        bio.style.height = bio.scrollHeight + 'px';
        requestAnimationFrame(function() {
          bio.classList.remove('is-open');
          bio.style.height = '0';
        });
        bio.addEventListener('transitionend', function handler() {
          bio.removeEventListener('transitionend', handler);
          card.open = false;
        });
      } else {
        card.open = true;
        var targetHeight = bio.scrollHeight;
        bio.style.height = '0';
        requestAnimationFrame(function() {
          bio.classList.add('is-open');
          bio.style.height = targetHeight + 'px';
        });
        bio.addEventListener('transitionend', function handler() {
          bio.removeEventListener('transitionend', handler);
          bio.style.height = 'auto';
        });
      }
    });
  })();
</script>
