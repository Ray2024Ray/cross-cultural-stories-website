---
layout: default
title: Home
permalink: /
---
# {{ site.podcast.name | default: "他乡与故乡 | Cross-cultural Stories" }}

{{ site.podcast.tagline | default: "跨文化的相遇与共鸣｜Stories of identity, belonging, and becoming" }}

<img src="{{ site.podcast.cover | default: '/images/podcast-cover.jpg' | relative_url }}" alt="Podcast Cover" style="max-width:220px;border-radius:12px;margin:12px 0;">

**订阅渠道：**  
- 🔊 [在 Spotify 收听]({{ site.podcast.spotify_show | default: 'https://open.spotify.com/show/6SNCpFk0GlnuIaLw8D3QGA' }})
{% if site.podcast.apple_show %}- 🍎 [Apple Podcasts]({{ site.podcast.apple_show }}){% endif %}
{% if site.podcast.xiaoyuzhou_show %}- 🌟 [小宇宙]({{ site.podcast.xiaoyuzhou_show }}){% endif %}

<iframe style="border-radius:12px;margin-top:12px" src="https://open.spotify.com/embed/show/6SNCpFk0GlnuIaLw8D3QGA?utm_source=generator" width="100%" height="152" frameborder="0" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

## 最新节目
{% assign latest = site.episodes | sort: "date" | reverse | slice: 0, 3 %}
{% if latest and latest.size > 0 %}
{% for ep in latest %}
- [{{ ep.title }}]({{ ep.url | relative_url }}) — {{ ep.date | date: "%Y-%m-%d" }} · {{ ep.duration }}
{% endfor %}
[查看全部节目 →]({{ "/episodes/" | relative_url }})
{% else %}
（还没有节目条目。先新增几期到 `site/collections/_episodes/`）
{% endif %}
