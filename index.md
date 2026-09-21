---
title: "Home"
---

<!-- Inline carousel-only styles (kept here so they don't clash with grid) -->
<style>
  .carousel { position: relative; overflow: hidden; }
  .carousel-track {
    display: flex;
    gap: 1rem;
    flex-wrap: nowrap;        /* keep in one row */
    overflow-x: auto;
    scroll-behavior: smooth;
    padding-bottom: .25rem;
    -ms-overflow-style: none; /* IE/Edge */
    scrollbar-width: none;    /* Firefox */
  }
  .carousel-track::-webkit-scrollbar { display: none; } /* WebKit */
  .carousel .card { flex: 0 0 300px; } /* slide width */
</style>

<section id="about" class="section">
  <div class="about-container">
    <img src="{{ '/assets/images/me.jpeg' | relative_url }}"
         alt="Michael Shoemaker"
         class="profile-pic">

    <div class="about-text">
      <h1>Hello World! I'm Michael Shoemaker</h1>
      <p>Senior Data Analyst | Teacher | Content Creator | .5x Programmer</p>
      <p>I build practical, production-like data engineering systems — orchestration, storage, transformations, serving, and observability — then explain the decisions behind them.</p>
      <p><strong>Core skills:</strong> Python · SQL · Linux · Airflow · Spark · BigQuery · Docker · GCP</p>

      <p class="social-links">
        <a href="https://www.linkedin.com/in/michaelshoemaker1" target="_blank" aria-label="LinkedIn">
          <i class="fa-brands fa-linkedin"></i>
        </a>
        <a href="https://www.youtube.com/@dataslinger6379" target="_blank" aria-label="YouTube">
          <i class="fa-brands fa-youtube"></i>
        </a>
      </p>
    </div>
  </div>
</section>

<!-- ===================== Projects ===================== -->
<section id="projects" class="section">
  <div class="section-header">
    <h2>🚀 Projects</h2>
    <a class="view-all" href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener">All repos →</a>
  </div>

  {% assign projects_count = site.data.projects | size %}
  {% if projects_count > 4 %}
    <div class="carousel">
      <button class="scroll-btn left" data-target="#projects-track" aria-label="Scroll projects left">‹</button>
      <div id="projects-track" class="carousel-track" role="region" aria-label="Projects list">
        {% for item in site.data.projects %}
        <article class="card">
          <a class="thumb" href="{{ item.link }}" target="_blank" rel="noopener" aria-label="Open project">
            <img src="{{ item.image | default: '/assets/images/placeholder_project.jpg' | relative_url }}"
                 alt="{{ item.title | escape }} thumbnail"
                 loading="lazy"
                 {% if item.preview_gif %}data-preview="{{ item.preview_gif | relative_url }}"{% endif %}>
          </a>
          <div class="card-body">
            <h3 class="card-title"><a href="{{ item.link }}" target="_blank" rel="noopener">{{ item.title }}</a></h3>
            <p class="card-text">{{ item.description }}</p>
            {% if item.stack %}<p class="card-tags">{{ item.stack }}</p>{% endif %}
            <div class="card-actions">
              {% if item.screenshot %}<a href="#" class="btn ghost" data-lightbox-src="{{ item.screenshot | relative_url }}">Preview</a>{% endif %}
              <a class="btn" href="{{ item.link }}" target="_blank" rel="noopener">Open</a>
            </div>
          </div>
        </article>
        {% endfor %}
      </div>
      <button class="scroll-btn right" data-target="#projects-track" aria-label="Scroll projects right">›</button>
    </div>
  {% else %}
    <div class="gallery">
      {% for item in site.data.projects %}
      <article class="card">
        <a class="thumb" href="{{ item.link }}" target="_blank" rel="noopener" aria-label="Open project">
          <img src="{{ item.image | default: '/assets/images/placeholder_project.jpg' | relative_url }}"
               alt="{{ item.title | escape }} thumbnail" loading="lazy">
        </a>
        <div class="card-body">
          <h3 class="card-title"><a href="{{ item.link }}" target="_blank" rel="noopener">{{ item.title }}</a></h3>
          <p class="card-text">{{ item.description }}</p>
          {% if item.stack %}<p class="card-tags">{{ item.stack }}</p>{% endif %}
          <div class="card-actions">
            {% if item.screenshot %}<a href="#" class="btn ghost" data-lightbox-src="{{ item.screenshot | relative_url }}">Preview</a>{% endif %}
            <a class="btn" href="{{ item.link }}" target="_blank" rel="noopener">Open</a>
          </div>
        </div>
      </article>
      {% endfor %}
    </div>
  {% endif %}
</section>

<!-- ===================== Videos ===================== -->
<section id="certificates" class="section">
  <div class="section-header">
    <h2>📜 Certifications</h2>
  </div>

  {% assign certificates_count = site.data.certificates | size %}
  {% if certificates_count > 4 %}
    <div class="carousel">
      <button class="scroll-btn left" data-target="#certificates-track" aria-label="Scroll certificates left">‹</button>
      <div id="certificates-track" class="carousel-track" role="region" aria-label="Certificates list">
        {% for item in site.data.certificates %}
        <article class="card">
          <a class="thumb" href="{{ item.link | default: '#' }}" target="_blank" rel="noopener" aria-label="View certificate">
            <img src="{{ item.image | default: '/assets/images/placeholder_certificate.jpg' | relative_url }}"
                 alt="{{ item.title | escape }} thumbnail"
                 loading="lazy">
          </a>
          <div class="card-body">
            <h3 class="card-title">
              {% if item.link %}
                <a href="{{ item.link }}" target="_blank" rel="noopener">{{ item.title }}</a>
              {% else %}
                {{ item.title }}
              {% endif %}
            </h3>
            {% if item.issuer %}<p class="card-text"><strong>Issuer:</strong> {{ item.issuer }}</p>{% endif %}
            {% if item.date %}<p class="card-text"><small>Issued: {{ item.date }}</small></p>{% endif %}
            {% if item.description %}<p class="card-text">{{ item.description }}</p>{% endif %}
            <div class="card-actions">
              {% if item.image %}<a href="#" class="btn ghost" data-lightbox-src="{{ item.image | relative_url }}">Preview</a>{% endif %}
              {% if item.link %}<a class="btn" href="{{ item.link }}" target="_blank" rel="noopener">Verify</a>{% endif %}
            </div>
          </div>
        </article>
        {% endfor %}
      </div>
      <button class="scroll-btn right" data-target="#certificates-track" aria-label="Scroll certificates right">›</button>
    </div>
  {% else %}
    <div class="gallery">
      {% for item in site.data.certificates %}
      <article class="card">
        <a class="thumb" href="{{ item.link | default: '#' }}" target="_blank" rel="noopener" aria-label="View certificate">
          <img src="{{ item.image | default: '/assets/images/placeholder_certificate.jpg' | relative_url }}"
               alt="{{ item.title | escape }} thumbnail" loading="lazy">
        </a>
        <div class="card-body">
          <h3 class="card-title">
            {% if item.link %}
              <a href="{{ item.link }}" target="_blank" rel="noopener">{{ item.title }}</a>
            {% else %}
              {{ item.title }}
            {% endif %}
          </h3>
          {% if item.issuer %}<p class="card-text"><strong>Issuer:</strong> {{ item.issuer }}</p>{% endif %}
          {% if item.date %}<p class="card-text"><small>Issued: {{ item.date }}</small></p>{% endif %}
          {% if item.description %}<p class="card-text">{{ item.description }}</p>{% endif %}
          <div class="card-actions">
            {% if item.image %}<a href="#" class="btn ghost" data-lightbox-src="{{ item.image | relative_url }}">Preview</a>{% endif %}
            {% if item.link %}<a class="btn" href="{{ item.link }}" target="_blank" rel="noopener">Verify</a>{% endif %}
          </div>
        </div>
      </article>
      {% endfor %}
    </div>
  {% endif %}
</section>

<!-- ===================== Articles ===================== -->
<section id="articles" class="section">
  <div class="section-header">
    <h2>✍️ Articles</h2>
    <a class="view-all" href="https://medium.com/@{{ site.medium_username }}" target="_blank" rel="noopener">Medium →</a>
  </div>

  {% assign articles_count = site.data.articles | size %}
  {% if articles_count > 4 %}
    <div class="carousel">
      <button class="scroll-btn left" data-target="#articles-track" aria-label="Scroll articles left">‹</button>
      <div id="articles-track" class="carousel-track" role="region" aria-label="Articles list">
        {% for item in site.data.articles %}
        <article class="card">
          <a class="thumb" href="{{ item.link }}" target="_blank" rel="noopener" aria-label="Open article">
            <img src="{{ item.image | default: '/assets/images/placeholder_article.jpg' | relative_url }}"
                 alt="{{ item.title | escape }} thumbnail"
                 loading="lazy"
                 {% if item.preview_gif %}data-preview="{{ item.preview_gif | relative_url }}"{% endif %}>
          </a>
          <div class="card-body">
            <h3 class="card-title"><a href="{{ item.link }}" target="_blank" rel="noopener">{{ item.title }}</a></h3>
            {% if item.subtitle %}<p class="card-text">{{ item.subtitle }}</p>{% endif %}
            <div class="card-actions">
              {% if item.screenshot %}<a href="#" class="btn ghost" data-lightbox-src="{{ item.screenshot | relative_url }}">Preview</a>{% endif %}
              <a class="btn" href="{{ item.link }}" target="_blank" rel="noopener">Read</a>
            </div>
          </div>
        </article>
        {% endfor %}
      </div>
      <button class="scroll-btn right" data-target="#articles-track" aria-label="Scroll articles right">›</button>
    </div>
  {% else %}
    <div class="gallery">
      {% for item in site.data.articles %}
      <article class="card">
        <a class="thumb" href="{{ item.link }}" target="_blank" rel="noopener" aria-label="Open article">
          <img src="{{ item.image | default: '/assets/images/placeholder_article.jpg' | relative_url }}"
               alt="{{ item.title | escape }} thumbnail" loading="lazy">
        </a>
        <div class="card-body">
          <h3 class="card-title"><a href="{{ item.link }}" target="_blank" rel="noopener">{{ item.title }}</a></h3>
          {% if item.subtitle %}<p class="card-text">{{ item.subtitle }}</p>{% endif %}
          <div class="card-actions">
            {% if item.screenshot %}<a href="#" class="btn ghost" data-lightbox-src="{{ item.screenshot | relative_url }}">Preview</a>{% endif %}
            <a class="btn" href="{{ item.link }}" target="_blank" rel="noopener">Read</a>
          </div>
        </div>
      </article>
      {% endfor %}
    </div>
  {% endif %}
</section>

<!-- Tiny helper script for arrow buttons -->
<script>
(function () {
  function init(btn) {
    var targetSel = btn.getAttribute('data-target');
    var track = document.querySelector(targetSel);
    if (!track) return;
    var step = Math.max(300, Math.floor(track.clientWidth * 0.9));

    btn.addEventListener('click', function () {
      track.scrollBy({ left: btn.classList.contains('left') ? -step : step, behavior: 'smooth' });
    });

    function update() {
      var max = track.scrollWidth - track.clientWidth - 1;
      var x = track.scrollLeft;
      var leftBtn = track.parentElement.querySelector('.scroll-btn.left');
      var rightBtn = track.parentElement.querySelector('.scroll-btn.right');
      if (leftBtn) leftBtn.disabled = x <= 0;
      if (rightBtn) rightBtn.disabled = x >= max;
    }
    track.addEventListener('scroll', update, { passive: true });
    window.addEventListener('resize', update);
    update();
  }
  document.querySelectorAll('.scroll-btn').forEach(init);
})();
</script>
