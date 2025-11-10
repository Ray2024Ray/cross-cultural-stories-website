---
layout: default
title: All episodes
permalink: /episodes/
---

<section class="section">
  <div class="container">
    <div class="section__info">
      <div class="section__head">
        <h2 class="section__title">All episodes</h2>
      </div>
    </div>
    <div class="row">
      {% assign eps = site.episodes | sort: 'date' | reverse %}
      {% for ep in eps %}
      <div class="col col-4 col-t-6 col-m-12">
        <article class="c-blog-card">
          <div class="c-blog-card__inner">
            <a class="c-blog-card__image" href="{{ ep.spotify | default: ep.external_url }}" target="_blank" rel="noopener">
              <img src="{{ ep.cover | default: '/images/podcast-cover.png' | relative_url }}" alt="{{ ep.title | escape }}">
            </a>
            <div class="c-blog-card__content">
              <h3 class="c-blog-card__title">
                <a href="{{ ep.spotify | default: ep.external_url }}" target="_blank" rel="noopener">{{ ep.title }}</a>
              </h3>
              {% if ep.excerpt %}<p class="c-blog-card__excerpt">{{ ep.excerpt }}</p>{% endif %}
            </div>
          </div>
        </article>
      </div>
      {% endfor %}
    </div>
  </div>
</section>
