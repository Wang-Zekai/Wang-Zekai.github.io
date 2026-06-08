---
permalink: /news/
title: "新闻"
author_profile: true
---

这里整理我的近期动态、科研进展和网站更新。

## 近期动态

- **2026.04**：整理“大模型强化学习与搜索推理”第一期科研轮转总结，系统梳理 PPO、GRPO 与 Search-R1 等方向。
- **2025.10**：发布新版 Archlab 课程实践记录。
- **2024.09**：进入北京大学信息科学技术学院学习。

## 最新文章

{% for post in site.posts limit:5 %}
- {{ post.date | date: "%Y-%m-%d" }}：[{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
