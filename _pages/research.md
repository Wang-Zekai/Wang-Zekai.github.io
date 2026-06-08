---
permalink: /research/
title: "研究"
author_profile: true
---

我的研究兴趣集中在大语言模型推理能力如何形成、如何被外部工具和检索过程增强，以及如何在复杂信息环境中保持可靠。

## 研究方向

### LLM Reasoning

关注大语言模型在复杂任务中的多步推理过程，包括长链推理、推理路径组织、答案形成机制，以及训练和推理阶段的行为差异。

### Retrieval and Tool-Augmented Reasoning

关注模型如何调用搜索、检索和外部工具，以及这些外部信息如何影响推理质量、回答稳定性和最终任务表现。

### Trustworthy LLMs

关注模型在错误知识、无关上下文和不稳定工具反馈下的鲁棒性，尤其是幻觉、错误知识干扰与推理可靠性问题。

### Interpretability

希望进一步学习 mechanistic interpretability 与 reasoning robustness 相关方法，从模型输出、训练日志和中间行为出发理解推理过程。

## 项目实践

### Multi-Agent Tool-Use RL

参与 multi-agent tool-use RL 项目实践，主要负责代码编写、实验运行与结果分析。该项目关注大语言模型在工具调用与多智能体协作场景下的推理优化问题，尤其是如何将最终任务表现合理分配到不同 agent、工具调用和推理步骤上。

相关工作包括：

- 参与 multi-agent 推理框架的实现与调试；
- 阅读、复现和分析 Search-R1 等检索增强推理与强化学习框架；
- 观察 EM / F1、search calls、finish ratio、response length 等指标；
- 分析搜索策略、奖励设计和回答质量之间的关系；
- 基于 verl / vLLM 相关训练与推理框架参与实验运行和问题排查。

## 研究记录

{% assign research_posts = site.posts | where_exp: "post", "post.categories contains 'research'" %}
{% if research_posts.size > 0 %}
{% for post in research_posts %}
- {{ post.date | date: "%Y-%m-%d" }}：[{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% else %}
更多研究记录会陆续整理。
{% endif %}
