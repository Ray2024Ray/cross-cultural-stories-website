---
layout: default
title: Home
permalink: /
---

<section class="c-hero">
  <div class="container">
    <div class="c-hero__inner row">
      <!-- 左侧：标题 + 文案 + 按钮 -->
      <div class="c-hero__left col col-6">
        <h1 class="c-hero__title">Cross-cultural Stories&nbsp;·&nbsp;他乡与故乡</h1>

        <div class="c-hero__description">
          <p>I’m Ray, a chemical engineer turned storyteller. 
          
          In this podcast, I talk to friends, family, and fellow travelers in Mandarin, English, or Korean about the things we bring with us—and the things we leave behind.

We explore cultural differences, identity shifts, everyday joy, and emotional struggles.

You may hear your own story in ours.</p>
        </div>
    
    <!-- 自动读取配置的订阅渠道 + 平台图标 -->
    <div class="subscribe-section" style="margin-top:28px;">
      <p style="font-weight:600;margin-bottom:10px;">订阅平台：</p>
      <div class="subscribe-buttons" style="display:flex;flex-wrap:wrap;gap:10px;justify-content:center;">
        {% if site.podcast.spotify_show %}
        <a class="c-button c-button--primary c-button--small" href="{{ site.podcast.spotify_show }}" target="_blank" rel="noopener">
          <img src="{{ '/images/spotify-icon.png' | relative_url }}" alt="Spotify" style="height:18px;vertical-align:middle;margin-right:6px;">Spotify
        </a>
        {% endif %}
    
        {% if site.podcast.apple_show %}
        <a class="c-button c-button--secondary c-button--small" href="{{ site.podcast.apple_show }}" target="_blank" rel="noopener">
          <img src="{{ '/images/apple-icon.png' | relative_url }}" alt="Apple Podcasts" style="height:18px;vertical-align:middle;margin-right:6px;">Apple Podcasts
        </a>
        {% endif %}
    
        {% if site.podcast.xiaoyuzhou_show %}
        <a class="c-button c-button--secondary c-button--small" href="{{ site.podcast.xiaoyuzhou_show }}" target="_blank" rel="noopener">
          <img src="{{ '/images/xiaoyuzhou-icon.png' | relative_url }}" alt="小宇宙" style="height:18px;vertical-align:middle;margin-right:6px;">小宇宙
        </a>
        {% endif %}
    
        {% if site.podcast.castbox_show %}
        <a class="c-button c-button--secondary c-button--small" href="{{ site.podcast.castbox_show }}" target="_blank" rel="noopener">
          <img src="{{ '/images/castbox-icon.png' | relative_url }}" alt="Castbox" style="height:18px;vertical-align:middle;margin-right:6px;">Castbox
        </a>
        {% endif %}
      </div>
    </div>

      </div>

     <!-- 右侧：封面图 -->
    <div class="c-hero__right col col-6">
      <div class="c-hero__image">
        <img src="{{ '/images/podcast-cover.png' | relative_url }}" alt="Cross-cultural Stories 封面">
      </div>
    </div>

    </div>
  </div>
</section>

<!-- Latest Episodes（先做 6 张卡片；后面我可以帮你换成自动读取） -->
<section class="section">
  <div class="container">
    <div class="section__info">
      <div class="section__head">
        <h2 class="section__title">Latest Episodes</h2>
        <a class="section__link" href="/episodes/">View all <i class="ion-md-arrow-forward"></i></a>
      </div>
      <div class="section__description">
        <p>最近更新的 6 期节目。</p>
      </div>
    </div>

    <div class="row">
      <!-- 复制这个卡片块 6 次，替换标题/简介/链接/封面图 -->
      <div class="col col-4 col-t-6 col-m-12">
        <article class="c-blog-card">
          <div class="c-blog-card__inner">
            <a class="c-blog-card__image" href="https://open.spotify.com/episode/你的ID" target="_blank" rel="noopener">
              <img src="{{ '/assets/images/ep016.jpg' | relative_url }}" alt="EP016">
            </a>
            <div class="c-blog-card__content">
              <div class="c-blog-card__tags-box">
                <span class="c-blog-card__tag">Podcast</span>
                <span class="c-blog-card__tag">Identity</span>
              </div>
              <h3 class="c-blog-card__title">
                <a href="https://open.spotify.com/episode/你的ID" target="_blank" rel="noopener">
                  EP016｜寻我之旅：一个中国女孩的全球漂流与扎根
                </a>
              </h3>
              <p class="c-blog-card__excerpt">在异国他乡更清晰地看见自己的来处与去处。</p>
            </div>
          </div>
        </article>
      </div>

      <!-- 示例卡片 2 -->
      <div class="col col-4 col-t-6 col-m-12">
        <article class="c-blog-card">
          <div class="c-blog-card__inner">
            <a class="c-blog-card__image" href="https://open.spotify.com/episode/7vqTCZjvrCChHvCa7rMN6P" target="_blank" rel="noopener">
              <img src="{{ '/assets/images/ep015.jpg' | relative_url }}" alt="EP015">
            </a>
            <div class="c-blog-card__content">
              <div class="c-blog-card__tags-box">
                <span class="c-blog-card__tag">Stanford</span>
                <span class="c-blog-card__tag">Volunteer</span>
              </div>
              <h3 class="c-blog-card__title">
                <a href="https://open.spotify.com/episode/7vqTCZjvrCChHvCa7rMN6P" target="_blank" rel="noopener">
                  EP015｜文化近距离 | 从斯坦福志愿者看跨文化连接
                </a>
              </h3>
              <p class="c-blog-card__excerpt">十年社区志愿经历里的相遇与陪伴。</p>
            </div>
          </div>
        </article>
      </div>

      <!-- 再复制 4 张卡片…（EP014 ~ EP011 或任意 4 期） -->
    </div>
  </div>
</section>
