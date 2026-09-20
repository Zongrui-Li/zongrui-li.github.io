---
layout: single
title: "About"
permalink: /en/
lang: en
---

I'm **Zongrui Li**. I received my bachelor's degree in Artificial Intelligence from Jilin University, and I'm now pursuing a PhD in Computer Science at Sun Yat-sen University.

My research focuses on **multi-agent coordination**, spanning multi-agent reinforcement learning, cooperative policy learning, and distributed decision-making — with the goal of enabling multiple agents to cooperate (and compete) to solve complex tasks that a single agent cannot handle alone.

## Contact

- **Email**: [lizr1122@mails.jlu.edu.cn](mailto:lizr1122@mails.jlu.edu.cn)
- **GitHub**: [github.com/Zongrui-Li](https://github.com/Zongrui-Li)

## Research Interests

- Multi-agent reinforcement learning (MARL)
- Cooperative policy learning and credit assignment
- Distributed decision-making

## Education

- **Sun Yat-sen University · PhD in Computer Science** (2027–present)  
  Research area: multi-agent coordination and multi-agent reinforcement learning.
- **Jilin University · B.Eng. in Artificial Intelligence** (2023–2027)  
  Coursework in machine learning, deep learning, reinforcement learning, and data structures & algorithms.

## Publications

{% assign publications = site.publications | sort: 'date' | reverse %}
{% if publications.size == 0 %}
No publications yet.
{% else %}
<ol>
{% for pub in publications %}
  <li><strong>{{ pub.title }}</strong>, {{ pub.authors }}, <em>{{ pub.venue }}</em>, {{ pub.date | date: "%Y" }}{% if pub.paperurl %}. <a href="{{ pub.paperurl }}" target="_blank" rel="noopener">Link</a>{% endif %}</li>
{% endfor %}
</ol>
{% endif %}

See the [Publications]({{ '/publications/' | relative_url }}) page for details.
