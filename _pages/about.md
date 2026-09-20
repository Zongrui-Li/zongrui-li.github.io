---
layout: single
title: "关于我"
permalink: /
lang: zh
---

我是**李宗睿（Zongrui Li）**，本科毕业于吉林大学人工智能专业，目前在中山大学计算机科学与技术专业攻读博士学位。

我的研究兴趣是**多智能体协同**，关注多智能体强化学习、协作策略学习与分布式决策，希望让多个智能体通过协作与博弈，共同解决单个智能体难以完成的复杂任务。

## 联系方式

- **邮箱**：[lizr1122@mails.jlu.edu.cn](mailto:lizr1122@mails.jlu.edu.cn)
- **GitHub**：[github.com/Zongrui-Li](https://github.com/Zongrui-Li)

## 研究兴趣

- 多智能体强化学习（MARL）
- 协作策略学习与信用分配
- 分布式决策

## 教育经历

- **中山大学 · 计算机科学与技术（博士）**（2027–至今）  
  研究方向：多智能体协同、多智能体强化学习。
- **吉林大学 · 人工智能（本科）**（2023–2027）  
  主修机器学习、深度学习、强化学习、数据结构与算法等。

## 发表论文

{% assign publications = site.publications | sort: 'date' | reverse %}
{% if publications.size == 0 %}
暂无论文。
{% else %}
<ol>
{% for pub in publications %}
  <li><strong>{{ pub.title }}</strong>，{{ pub.authors }}，<em>{{ pub.venue }}</em>，{{ pub.date | date: "%Y" }}{% if pub.paperurl %}。<a href="{{ pub.paperurl }}" target="_blank" rel="noopener">链接</a>{% endif %}</li>
{% endfor %}
</ol>
{% endif %}

更多详情见 [发表论文]({{ '/publications/' | relative_url }}) 页面。
