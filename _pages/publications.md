---
layout: single
title: "发表论文"
permalink: /publications/
---

{% assign publications = site.publications | sort: 'date' | reverse %}
{% if publications.size == 0 %}
<p>暂无论文。</p>
{% else %}
<ul class="publications">
  {% for pub in publications %}
    <li class="publication">
      <h2 class="publication__title">{{ pub.title }}</h2>
      <p class="publication__authors">{{ pub.authors }}</p>
      <p class="publication__meta">{{ pub.venue }}{% if pub.date %} · {{ pub.date | date: "%Y-%m" }}{% endif %}</p>
      <div class="publication__links">
        {% if pub.paperurl %}<a href="{{ pub.paperurl }}" target="_blank" rel="noopener">论文</a>{% endif %}
        {% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}" target="_blank" rel="noopener">DOI</a>{% endif %}
        <a href="{{ pub.url | relative_url }}">详情</a>
      </div>
    </li>
  {% endfor %}
</ul>
{% endif %}
