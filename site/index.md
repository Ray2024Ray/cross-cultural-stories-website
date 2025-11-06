
---
# {{ site.podcast.name }}

{{ site.podcast.tagline }}

<img src="{{ site.podcast.cover | relative_url }}" alt="Podcast Cover" style="max-width:220px;border-radius:12px;margin:12px 0;">

**订阅渠道：**  
- 🔊 [在 Spotify 收听]({{ site.podcast.spotify_show }})  
{% if site.podcast.apple_show %}- 🍎 [在 Apple Podcasts 收听]({{ site.podcast.apple_show }}){% endif %}
{% if site.podcast.xiaoyuzhou_show %}- 🌟 [在小宇宙收听]({{ site.podcast.xiaoyuzhou_show }}){% endif %}

<!-- Spotify 节目级播放器（展示整档 Show） -->
<iframe style="border-radius:12px;margin-top:12px" src="https://open.spotify.com/embed/show/6SNCpFk0GlnuIaLw8D3QGA?utm_source=generator" width="100%" height="152" frameborder="0" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

## 最新节目
{% assign latest = site.episodes | sort: "date" | reverse | slice: 0, 3 %}
{% if latest and latest.size > 0 %}
{% for ep in latest %}
- [{{ ep.title }}]({{ ep.url | relative_url }}) — {{ ep.date | date: "%Y-%m-%d" }} · {{ ep.duration }}
{% endfor %}
[查看全部节目 →]({{ "/episodes/" | relative_url }})
{% else %}
（还没有节目条目。请先按下面“第 4 步”新增几期。）
{% endif %}

---

# 他乡与故乡 · Cross-cultural Stories
一档关于“他乡与故乡、身份与连接”的跨文化播客。

[查看全部节目 →]({{ "/episodes/" | relative_url }})
