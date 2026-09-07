---
layout: single
title: "简历 / CV"
permalink: /cv/
---

## 基本信息

- **姓名**：李宗睿（Zongrui Li）
- **邮箱**：[lizr1122@mails.jlu.edu.cn](mailto:lizr1122@mails.jlu.edu.cn)
- **GitHub**：[github.com/Zongrui-Li](https://github.com/Zongrui-Li)

## 教育经历

- **中山大学 · 计算机科学与技术（博士）**（2027–至今）
- **吉林大学 · 人工智能（本科）**（2023–2027）

## 研究兴趣

多智能体协同、多智能体强化学习、协作策略学习、分布式决策。

## 发表论文

{% assign publications = site.publications | sort: 'date' | reverse %}
{% for pub in publications %}
1. **{{ pub.title }}**，{{ pub.authors }}，*{{ pub.venue }}*，{{ pub.date | date: "%Y" }}。[链接]({{ pub.paperurl }})
{% endfor %}
