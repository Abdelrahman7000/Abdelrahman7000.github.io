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
    <div class="about-text">
      <h1>Hello World! I'm Abdelrahman Shaban</h1>
      <p>Data Engineer | Analytics Engineer</p>
      <p>I build practical, data pipelines — orchestration, storage, transformations, and serving — to drive business-critical data engineering projects.</p>
      
      <p><strong>Core skills:</strong></p>
      <ul class="skills-list" style="list-style: none; padding: 0; display: flex; flex-wrap: wrap; gap: 0.75rem; align-items: center;">
        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python logo" width="18" height="18">
          Python
        </li>
        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/azuresqldatabase/azuresqldatabase-original.svg" alt="SQL logo" width="18" height="18">
          SQL
        </li>
        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" alt="Linux logo" width="18" height="18">
          Linux
        </li>
        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/apacheairflow/apacheairflow-original.svg" alt="Airflow logo" width="18" height="18">
          Airflow
        </li>
       <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/apachespark/apachespark-original.svg" alt="PySpark logo" width="18" height="18">
          PySpark
        </li>
        
        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" alt="Docker logo" width="18" height="18">
          Docker
        </li>

        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/npm/simple-icons@11.15.0/icons/dbt.svg" alt="dbt logo" width="18" height="18">
          dbt
        </li>

        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/npm/simple-icons@v11/icons/alteryx.svg" alt="Alteryx logo" width="18" height="18" style="filter: invert(1);">
          Alteryx
        </li>

        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" alt="PostgreSQL logo" width="18" height="18">
          PostgreSQL
        </li>
        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/npm/simple-icons@v11/icons/snowflake.svg" alt="Snowflake logo" width="18" height="18" style="filter: invert(1);">
          Snowflake
        </li>

        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-plain-wordmark.svg" alt="AWS logo" width="18" height="18" style="filter: invert(1);">
          AWS
        </li>

        <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/terraform/terraform-original.svg" alt="Terraform logo" width="18" height="18">
          Terraform basics
        </li>

         <li style="display: flex; align-items: center; gap: 0.35rem; background: rgba(255,255,255,0.05); padding: 0.35rem 0.65rem; border-radius: 6px; border: 1px solid rgba(255,255,255,0.1);">
          <img src="https://cdn.jsdelivr.net/npm/simple-icons@11.15.0/icons/tableau.svg" alt="Terraform logo" width="18" height="18">
          Tableau basics
        </li>
      </ul>

      <p class="social-links" style="margin-top: 1.5rem;">
        <a href="https://www.linkedin.com/in/abdelrahman-shaban-41607b167/" target="_blank" aria-label="LinkedIn">
          <i class="fa-brands fa-linkedin"></i>
        </a>
       <a href="https://public.tableau.com/app/profile/abdelrahman.shaban/vizzes" target="_blank" aria-label="Tableau">
          <i class="fa-solid fa-chart-line"></i>
       </a>
      </p>
    </div>
  </div>
</section>

<!-- =====================Experience ========================-->
<style>
/* Work Experience Timeline */
.experience-timeline {
  position: relative;
  max-width: 900px;
  margin: 2rem auto 0;
  padding-left: 2rem;
  border-left: 2px solid rgba(255, 255, 255, 0.15);
}

.timeline-item {
  position: relative;
  margin-bottom: 2.5rem;
}

.timeline-item:last-child {
  margin-bottom: 0;
}

.timeline-dot {
  position: absolute;
  left: -2.55rem;
  top: 1.25rem;
  width: 14px;
  height: 14px;
  border-radius: 50%;
  background-color: #3b82f6;
  border: 3px solid #121212;
}

.timeline-content {
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 10px;
  padding: 1.5rem;
}

.experience-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: 0.75rem;
}

.job-title {
  margin: 0;
  font-size: 1.25rem;
  font-weight: 600;
  color: #ffffff;
}

.company-name {
  font-size: 1rem;
  color: #3b82f6;
  font-weight: 500;
}

.location {
  font-size: 0.9rem;
  color: #a0aec0;
}

.date-badge {
  background: rgba(255, 255, 255, 0.08);
  color: #e2e8f0;
  padding: 0.25rem 0.75rem;
  border-radius: 20px;
  font-size: 0.85rem;
  font-weight: 500;
}

.job-summary {
  font-size: 0.95rem;
  color: #cbd5e1;
  margin-bottom: 0.75rem;
}

.duties-list {
  margin: 0.5rem 0 1rem 1.2rem;
  padding: 0;
  color: #cbd5e1;
  font-size: 0.95rem;
  line-height: 1.6;
}

.duties-list li {
  margin-bottom: 0.4rem;
}

.tech-stack-pills {
  display: flex;
  flex-wrap: wrap;
  gap: 0.4rem;
  margin-top: 1rem;
}

.tech-pill {
  font-size: 0.75rem;
  background: rgba(59, 130, 246, 0.15);
  color: #60a5fa;
  border: 1px solid rgba(59, 130, 246, 0.3);
  padding: 0.15rem 0.5rem;
  border-radius: 4px;
}

@media (max-width: 600px) {
  .experience-header {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>

<section id="experience" class="section">
  <div class="section-header">
    <h2>💼 Work Experience</h2>
  </div>

  <div class="experience-timeline">
    {% for job in site.data.experience %}
    <div class="timeline-item">
      <div class="timeline-dot"></div>
      <div class="timeline-content card">
        <div class="experience-header">
          <div>
            <h3 class="job-title">{{ job.title }}</h3>
            <span class="company-name">{{ job.company }}</span>
            {% if job.location %}<span class="location"> • {{ job.location }}</span>{% endif %}
          </div>
          <span class="date-badge">{{ job.period }}</span>
        </div>

        {% if job.summary %}
          <p class="job-summary">{{ job.summary }}</p>
        {% endif %}

        {% if job.responsibilities %}
        <ul class="duties-list">
          {% for duty in job.responsibilities %}
            <li>{{ duty }}</li>
          {% endfor %}
        </ul>
        {% endif %}

        {% if job.tech_stack %}
        <div class="tech-stack-pills">
          {% for tech in job.tech_stack %}
            <span class="tech-pill">{{ tech }}</span>
          {% endfor %}
        </div>
        {% endif %}
      </div>
    </div>
    {% endfor %}
  </div>
</section>




<!-- ===================== Certificates ===================== -->
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



<!-- ===================== Articles ===================== -->
<!-- <section id="articles" class="section">
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
</section> -->



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
