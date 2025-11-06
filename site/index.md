# 他乡与故乡 · Things I Took With Me
一档关于“他乡与故乡、身份与连接”的跨文化播客。

## 最新节目
{% assign latest = site.episodes | sort: "date" | reverse | slice: 0, 3 %}
{% for ep in latest %}
- [{{ ep.title }}]({{ ep.url | relative_url }}) — {{ ep.date | date: "%Y-%m-%d" }} · {{ ep.duration }}
{% endfor %}

[查看全部节目 →]({{ "/episodes/" | relative_url }})
