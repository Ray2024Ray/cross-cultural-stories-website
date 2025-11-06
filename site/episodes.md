---
title: 所有节目
layout: default
permalink: /episodes/
---
<h1>所有节目</h1>
<ul class="episodes">
  {% assign eps = site.episodes | sort: "date" | reverse %}
  {% for ep in eps %}
    <li style="margin:14px 0;">
      <a href="{{ ep.url | relative_url }}">
        {% if ep.cover %}<img src="{{ ep.cover | relative_url }}" alt="{{ ep.title }}" style="max-width:220px;display:block;margin-bottom:6px;">{% endif %}
        <strong>{{ ep.title }}</strong><br>
        {{ ep.date | date: "%Y-%m-%d" }} · {{ ep.duration }}<br>
        {{ ep.excerpt }}
      </a><br>
      {% if ep.spotify %}<a href="{{ ep.spotify }}" target="_blank">Spotify</a>{% endif %}
    </li>
  {% endfor %}
</ul>
