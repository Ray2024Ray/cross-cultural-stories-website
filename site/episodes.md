---
title: 所有节目
layout: default
permalink: /episodes/
---

# 所有节目

{% assign eps = site.episodes | sort: "date" | reverse %}
{% for ep in eps %}
<div style="margin: 16px 0 20px;">
  <a href="{{ ep.url | relative_url }}" style="text-decoration:none;">
    {% if ep.cover %}
      <img src="{{ ep.cover | relative_url }}" alt="{{ ep.title }}" style="max-width:220px;border-radius:12px;display:block;margin-bottom:6px;">
    {% endif %}
    <strong>{{ ep.title }}</strong><br>
    <small>{{ ep.date | date: "%Y-%m-%d" }} · {{ ep.duration }}</small><br>
    <span style="color:#666">{{ ep.excerpt }}</span>
  </a>
</div>
{% endfor %}
