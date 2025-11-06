---
title: Episodes
layout: default
permalink: /en/episodes/
---
# Episodes (EN)
{% assign eps = site.episodes | where: "lang", "en" | sort: "date" | reverse %}
{% for ep in eps %}
- [{{ ep.title }}]({{ ep.url | relative_url }}) — {{ ep.date | date: "%b %d, %Y" }} · {{ ep.duration }}
{% endfor %}
