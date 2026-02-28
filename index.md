---
layout: default
---

# {{ site.title }}

{{ site.description }}

## 最新文章

{% for post in site.posts limit: 5 %}
### [{{ post.title }}]({{ post.url }})
<small>{{ post.date | date: "%Y-%m-%d" }}</small>

{{ post.excerpt | strip_html | truncate: 200 }}

{% endfor %}

## 关于

**GitHub 商机挖掘系统（GOMS）** 是一个自动发现 GitHub 高价值项目并生成商业分析和产品设计报告的系统。

### 核心功能

1. **GitHub 趋势监控** - 每日自动查询 Top 10 项目
2. **商业分析** - 深入分析商业可行性
3. **产品设计** - 定义 MVP 功能和定价策略
4. **Landing Page 生成** - 自动生成营销页面
5. **博客生成** - 自动生成知识库文章

### 仓库

- [Zoe Blog](https://github.com/qqqzhch/zoe-blog)
- [Zoe Landing Pages](https://github.com/qqqzhch/zoe-landing-pages)
